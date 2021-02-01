# ReflexOntology

The ReflexOntology and its Pituitary Dysfunction extension with two reflex rules as shown in the AIME 2021 submission.

Some notes:
- Due to limitations of SWRL (and OWL), some expressions are not as elegant as they could be; i.e., where we had to resort to explicly enumerating the tests associated with a reflex rule or follow-up rule.
- Due to apparent limitations of the Pellet reasoner, the `swrlb:subtract` builtin is not supported; hence, currently we explicitly state that a test-pattern of stage 2 can be triggered when a follow-up rule of stage 1 was triggered; a test-pattern of stage 3 can be triggered when a follow-up rule of stage 2 was triggered; and so on.

In future work, we aim to use a more expressive Semantic Web formalism such as <a href="https://github.com/w3c/N3">Notation3</a> with its range of builtins, support for (scoped) negation as failure and universal quantification.