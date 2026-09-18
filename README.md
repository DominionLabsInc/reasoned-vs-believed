# Reasoned vs. Believed

**The two ways a cognitive substrate knows, and the discipline that keeps them honest.**

Stefan Ragland, Dominion Labs Research & Development. Published 24 March 2026.

- Paper (PDF): [`paper/reasoned-vs-believed.pdf`](paper/reasoned-vs-believed.pdf)
- Paper (web): <https://dmnlabs.org/research/reasoned-vs-believed/>
- Contact: research@dmnlabs.org

## The argument

A substrate that accumulates knowledge knows in two ways. It **derives**, walking the structure it has
learned, and it **believes**, holding graded posteriors formed from evidence it was given. These are
different faculties with different failure modes, and where they diverge the divergence is diagnostic.

KNOW-50 observes the gap directly: it asks the running substrate fifty questions drawn from what it was
taught, withholds every answer, and records both what it reasons and what it believes, with the
derivation. Unconstrained derivation over an uncurated structure over-generates; bounded derivation can
fall short of a fact the system already believes. Four principles follow, and a substrate held to them
answers only what it can ground and abstains on the rest.

## The measurements

| What | Result | Data |
|---|---|---|
| KNOW-50, re-run 18 September 2026 | 37 of 37 correct on the questions it chose to answer, 13 honest abstentions, zero language model calls | [`data/know-50.json`](data/know-50.json) |
| Asserting when the evidence admits several hypotheses | asserting on any one of them gives 26 assertions of false cases out of 192; asserting only what all of them support gives 0, while still reaching 73% of true cases | [`data/assertion-under-ambiguity.json`](data/assertion-under-ambiguity.json) |
| An abstention that states its own remedy | the case the substrate asks for closes the ambiguity in 16 of 16 inductions, in a mean of 2.6 rounds; randomly chosen examples close 1 of 16 | [`data/closing-the-ambiguity.json`](data/closing-the-ambiguity.json) |

Each file is the manifest its run wrote, unedited. The ambiguity studies are reported in full in a
companion paper ([repository](https://github.com/DominionLabsInc/perceive-induce-name),
[paper](https://dmnlabs.org/research/perceive-induce-name/)).

## Citation

```bibtex
@techreport{ragland2026reasoned,
  title       = {Reasoned vs. Believed: the two ways a cognitive substrate knows},
  author      = {Ragland, Stefan},
  institution = {Dominion Labs},
  year        = {2026},
  month       = {3},
  url         = {https://dmnlabs.org/research/reasoned-vs-believed/}
}
```

## License

The paper and the data are released under [Creative Commons Attribution 4.0](LICENSE). Please cite the
paper if you use them.
