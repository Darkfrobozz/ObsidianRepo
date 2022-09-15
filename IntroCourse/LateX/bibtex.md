This is a system to handle references.
Provide a seperate document with the end '.bib'. In this document, provide your references. This is the syntax:

@misc{MultiRust,
title = {Multirust},
author = {Brian Anderson and others},
howpublished = "\url{https://github.com/brson/multirust}",
note = {visited on 2016-04-27}
}

@book{Tanenbaum2006,
author={Tanenbaum, Andrew S. and Woodhull, Albert S.},
title={Operating systems : design and implementation},
publisher={Pearson Prentice Hall},
address={Upper Saddle River, NJ},
year=2006,
edition={3. ed.},
isbn={0-13-142938-8 (korr.) (inb.)}
}





Moreover, these commands can be used in unision:

- \cite{reference}
- \bibliographystyle{plain}
- \bibliography{reference.bib}
