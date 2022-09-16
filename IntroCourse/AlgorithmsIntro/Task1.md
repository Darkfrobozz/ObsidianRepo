1. Length(L) - beräknar längden av listan L 
2. Count(x, L) - beräknar antalet förekomster av elementet x i listan L 
3. Member(x, L) - avgör om elementet x finns i listan L 
4. Last(L) - det sista elementet i listan L 
5. Append(A, B) - sätter ihop listorna A och B med A först.


1. Algoritm:
	1. Är lista empty?
		1. True -> retunera 0
		2. False -> hugg av huvud och retunera 1 + length av L
2. Algo: 
	1. Är lista empty?
		1. True -> retunera 0
		2. False -> är head x? + step 1
3. Algo:
	1. returnera 2. Algo > 0?
4. //impossible algorithm? Algo(L):
	1. Is empty?
		1. True -> Return Null
		2. False -> spara head i x och sen hugg och spara 4. Algo(L) i y
	2. Is y = Null
		1. True return x
		2. False return y
5. Algo(A, B)
	1. Is empty(A)
		1. True -> Sluta algoritmen här
		2. False -> spara head i x, hugg och kör Algo(A, B)
	2. Cons(x, B) ## lista B borde nu vara A + B med A först