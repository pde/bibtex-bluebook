This is a very unmaintained, very incomplete BibTex/LaTeX implementation of
the crazily complex Bluebook citation format used in US legal publication.

It was derived from the older inline BibTex file written by René Seindal.

It has a few cool features, most notably that it can automate _supra_ and _Id_
citations in footnotes. It also has numerous handy abevations, both for
signalling text, such as: `\See`, `\see`, `\seeeg`, `\Seeeg`, `\Cf`, `\cf`,
and for marking entries in bibliography files to be abbreviated, such as:
`\Journal \bibof \Contemporary \Tech`. Citations look like this:

```
\footnote{\See \cite{machlup50controversy}. But these debates built on an
older intellectual tradition; \seeeg \cite[at~191]{macleod88inventing}.}
```

Some major caveats you should bear in mind before using:

* **Law review articles may demand submissions in Word format**. If your use case
  might require Word, writing in LaTeX is a bad idea
* Large documents may in some cases require recompiling LaTeX to increase
  stack size
* These are antique and unmaintained files. Be prepared to edit and fix them,
  and in general to build your own house.
