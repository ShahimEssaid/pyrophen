.. _rstexamplejson:

##############
Example (JSON)
##############

pyrophen outputs the codeset in XML or JSON format. See :ref:`rstexamplexml` for XML.

The test class ``HpoFhirTerminologyApplicationTests`` writes a temporary file with the CodeSystem created for a small excerpt of the HPO located
in ``src/test/resources/hp_head.obo``.


This is the JSON file that is produced.


.. code-block:: bash

    {
      "resourceType": "CodeSystem",
      "id": "hpo",
      "url": "http://purl.obolibrary.org/obo/hp.fhir",
      "version": "http://purl.obolibrary.org/obo/hp/releases/2017-04-13/hp.owl",
      "name": "HPO",
      "title": "Human Phenotype Ontology Coding",
      "status": "active",
      "experimental": false,
      "date": "2021-05-03T08:04:39-04:00",
      "publisher": "The Human Phenotype Ontology",
      "contact": [ {
        "name": "Peter N. Robinson"
      } ],
      "description": "A FHIR code system representation of the Human Phenotype Ontology.",
      "purpose": "To provide a standardized vocabulary of human phenotypes encountered in human disease in a FHIR context.",
      "copyright": "https://hpo.jax.org/app/license",
      "concept": [ {
        "code": "HP:0000001",
        "display": "All"
      }, {
        "code": "HP:0040282",
        "display": "Frequent",
        "definition": "Present in 30% to 79% of the cases.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Frequent (79-30%)"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0040279"
        } ]
      }, {
        "code": "HP:0040281",
        "display": "Very frequent",
        "definition": "Present in 80% to 99% of the cases.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Very frequent (99-80%)"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0040279"
        } ]
      }, {
        "code": "HP:0040284",
        "display": "Very rare",
        "definition": "Present in 1% to 4% of the cases.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Very rare (<4-1%)"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Very rare (&lt;4-1%)"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0040279"
        } ]
      }, {
        "code": "HP:0040283",
        "display": "Occasional",
        "definition": "Present in 5% to 29% of the cases.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Occasional (29-5%)"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0040279"
        } ]
      }, {
        "code": "HP:0040280",
        "display": "Obligate",
        "definition": "Always present, i.e. in 100% of the cases.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Obligate (100%)"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0040279"
        } ]
      }, {
        "code": "HP:0100886",
        "display": "Abnormality of globe location",
        "definition": "An abnormality in the placement of the ocular globe (eyeball).",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of eyeball position"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of globe position"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of eyeball location"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0012374"
        } ]
      }, {
        "code": "HP:0012374",
        "display": "Abnormal globe morphology",
        "definition": "An anomaly of the eyeball.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of the globe"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0012372"
        } ]
      }, {
        "code": "HP:0040279",
        "display": "Frequency",
        "definition": "Class to represent frequency of phenotypic abnormalities within a patient cohort.",
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000001"
        } ]
      }, {
        "code": "HP:0100887",
        "display": "Abnormality of globe size",
        "definition": "An abnormality in the size of the ocular globe (eyeball).",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Eye size difference"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of eyeball size"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0012374"
        } ]
      }, {
        "code": "HP:0000528",
        "display": "Anophthalmia",
        "definition": "Absence of the globe or eyeball.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "No globe of eye"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Clinical anophthalmia, unilateral/bilateral"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Absence of eyeballs"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Missing eyeball"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Missing globe of eye"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Absence of globes of eyes"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Ocular absence"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "No eyeball"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Anophthalmia, clinical"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Failure of development of eyeball"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0100887"
        } ]
      }, {
        "code": "HP:0040285",
        "display": "Excluded",
        "definition": "Present in 0% of the cases.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Excluded (0%)"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0040279"
        } ]
      }, {
        "code": "HP:0012372",
        "display": "Abnormal eye morphology",
        "definition": "A structural anomaly of the eye.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormal eye morphology"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormally shaped eye"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000478"
        } ]
      }, {
        "code": "HP:0012373",
        "display": "Abnormal eye physiology",
        "definition": "A functional anomaly of the eye.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormal eye physiology"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000478"
        } ]
      }, {
        "code": "HP:0000118",
        "display": "Phenotypic abnormality",
        "definition": "A phenotypic abnormality.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Organ abnormality"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000001"
        } ]
      }, {
        "code": "HP:0000007",
        "display": "Autosomal recessive inheritance",
        "definition": "A mode of inheritance that is observed for traits related to a gene encoded on one of the autosomes (i.e., the human chromosomes 1-22) in which a trait manifests in homozygotes. In the context of medical genetics, autosomal recessive disorders manifest in homozygotes (with two copies of the mutant allele) or compound heterozygotes (whereby each copy of a gene has a distinct mutant allele).",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Autosomal recessive predisposition"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Autosomal recessive"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Autosomal recessive form"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000005"
        } ]
      }, {
        "code": "HP:0000568",
        "display": "Microphthalmia",
        "definition": "A developmental anomaly characterized by abnormal smallness of one or both eyes.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Nanophthalmos"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormally small globe of eye"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Decreased size of eyeball"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormally small eyeball"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Microphthalmos"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Decreased size of globe of eye"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0100887"
        } ]
      }, {
        "code": "HP:0007686",
        "display": "Abnormal pupillary function",
        "definition": "A functional abnormality of the pupil.",
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0012373"
        } ]
      }, {
        "code": "HP:0000006",
        "display": "Autosomal dominant inheritance",
        "definition": "A mode of inheritance that is observed for traits related to a gene encoded on one of the autosomes (i.e., the human chromosomes 1-22) in which a trait manifests in heterozygotes. In the context of medical genetics, an autosomal dominant disorder is caused when a single copy of the mutant allele is present. Males and females are affected equally, and can both transmit the disorder with a risk of 50% for each child of inheriting the mutant allele.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Autosomal dominant type"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Autosomal dominant"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Autosomal dominant form"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000005"
        } ]
      }, {
        "code": "HP:0000478",
        "display": "Abnormality of the eye",
        "definition": "Any abnormality of the eye, including location, spacing, and intraocular abnormalities.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of the eye"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormal eye"
        }, {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Eye disease"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000118"
        } ]
      }, {
        "code": "HP:0000632",
        "display": "Lacrimation abnormality",
        "definition": "Abnormality of tear production.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Abnormality of tear production"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0012373"
        } ]
      }, {
        "code": "HP:0000005",
        "display": "Mode of inheritance",
        "definition": "The pattern in which a particular genetic trait or disorder is passed from one generation to the next.",
        "designation": [ {
          "use": {
            "system": "http://snomed.info/sct",
            "code": "900000000000013009",
            "display": "Synonym (core metadata concept)"
          },
          "value": "Inheritance"
        } ],
        "property": [ {
          "code": "parent",
          "valueCode": "HP:0000001"
        } ]
      } ]
    }
