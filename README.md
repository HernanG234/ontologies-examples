# Ontologies examples #

Aquí se encuentran ejemplos resueltos de ontologías, como referencia para ser usados en la materia **Técnicas de la Inteligencia Artificial** de la carrera de **Ing. Electrónica** de la **Facultad de Cs. Exactas, Ingnenierías y Agrimensura** de la **Universidad Nacional de Rosario**.

Principalmente se encuentran resoluciones paso a paso de los tutoriales de la Universidad de Manchester:
* [A Practical Guide To Building OWL Ontologies](http://owl.cs.manchester.ac.uk/publications/talks-and-tutorials/protg-owl-tutorial/) (The pizza one)
* [Manchester Family History Advanced OWL](http://owl.cs.manchester.ac.uk/publications/talks-and-tutorials/fhkbtutorial/) (FHKB)
* Ejemplo enfocado a la carrera (A DEFINIR)

## Observaciones sobre la FHKB ##

If you have done all the tasks within this tutorial, then you will have touched most parts of OWL 2. Unusually for most uses of OWL we have concentrated on individuals, rather than just on the TBox. One note of warning – the full FHKB has some 450 members of the Bright family and takes a reasonably long time to classify, even on a sensible machine. The FHKB is not scalable in its current form.

One reason for this is that we have deliberately maximised inference. We have attempted not to explicitly type the individuals, but drive that through domain and range constraints. We are making the property hierarchy do lots of work. For the individual Robert David Bright, we only have a couple of assertions, but we infer some 1 500 facts between Robert David Bright and other named individuals in the FHKB, displaying this in Protégé causes problems. We have various complex classes in the TBox and so on.

We probably do not wish to drive a genealogical application using an FHKB in this form. Its purpose is educational. It touches most of OWL 2 and shows a lot of what it can do, but also a considerable amount of what it cannot do. As inference is maximised, the FHKB breaks most of the OWL 2 reasoners at the time of writing. However, it serves its role to teach about OWL 2.

OWL 2 on its own and using it in this style, really does not work for family history. We have seen that siblings and cousins cause problems. rules in varius forms can do this kind of thing easily—it is one of the primary examples for learning about Prolog. Nevertheless, the FHKB does show how much inference between named individuals can be driven from a few fact assertions and a property hierarchy. Assuming a powerful enough reasoner and the ability to deal with many individuals, it would be possible to make a family history application using the FHKB; as long as one hid the long and sometimes complex queries and manipulations that would be necessary to ‘prune’ some of the ‘extra’ facts found about individuals. However, the FHKB does usefully show the power of OWL 2, touch a great deal of the language and demonstrate some of its limitations.
