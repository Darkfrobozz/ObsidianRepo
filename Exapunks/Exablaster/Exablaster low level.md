As seen in [[Exablaster Highest level]], we dial a number, get a new number from the file in those [[Hosts]] and dial those numbers.
- Dial number from file 300
	- Traverse link 800
	- Copy number from file 200 to 300
	- traverse -1
	- dial -1
	- Dial new number
- Repeat 

We will use two [[Exas]] to copy number from file, we need not worry about getting back to the same host because a phone number will never be found again.

GRAB 300
LINK 800

MARK DIALLOOP
COPY F #DIAL
TEST EOF
FJMP DIALLOOP

LINK 800
REPL COPIER
SEEK -9999

MARK COPYLOOP
COPY M F
TEST EOF
FJMP COPYLOOP

KILL
LINK -1
SEEK -9999
COPY -1 #DIAL
JUMP DIALLOOP


MARK COPIER
GRAB 200
SEEK 1
MARK COPIERLOOP
COPY F M
JUMP COPIERLOOP

Problem with current solution! Connection Refused?? Some numbers are bad...
We need Exa to try number, fail then next one to try. We can use the fact that a phone number is always 11 digits to copy more than just the first number.

Special starting case, all cases have name except starting one

We have a concrete way to dial but we need to be able to explore all the phones and they will branch like a tree [[PhoneTree]]. Solution:

GRAB 300
LINK 800
COPY 11 X
JUMP DIALLOOP

MARK COMPLEXDIALLING
NOTE LETS JUST VOID
NOTE THE NUMBERS WE HAVE
NOTE CALLED
NOTE BEFORE COPYING VOID
NOTE LAST 12
SEEK -9999
TEST EOF
TJMP DONE
COPY -1 #DIAL
COPY 12 X
MARK DIALLOOP
COPY F #DIAL
NOTE VOID HERE
SEEK -1
VOID F
SUBI X 1 X
TEST X = 0
FJMP DIALLOOP


REPL COPIER

NOOP
SEEK 9999
NOOP
NOOP

MARK COPYLOOP
TEST MRD
FJMP COMPLEXDIALLING
COPY M F
NOOP
JUMP COPYLOOP

MARK COPIER
LINK 800
GRAB 200

MARK COPIERLOOP
COPY F M
TEST EOF
FJMP COPIERLOOP
HALT

MARK DONE
WIPE
HALT

