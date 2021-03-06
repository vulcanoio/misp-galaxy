# misp-galaxy

[![Build Status](https://travis-ci.org/MISP/misp-galaxy.svg?branch=master)](https://travis-ci.org/MISP/misp-galaxy)

MISP galaxy is a simple method to express a large object called cluster that can be attached to MISP events or
attributes. A cluster can be composed of one or more elements. Elements are expressed as key-values. There
are default vocabularies available in MISP galaxy but those can be overwritten, replaced or updated as you wish.

Existing clusters and vocabularies can be used as-is or as a template. MISP distribution can be applied
to each cluster to permit a limited or broader distribution scheme.

Vocabularies are from existing standards (like STIX, Veris, MISP and so on) or custom ones.

The objective is to have a comment set of clusters for organizations starting analysis but that can be expanded
to localized information (which is not shared) or additional information (that can be shared).

# Available clusters

- [clusters/threat-actors.json](clusters/threat-actors.json) - Adversary groups - Known or estimated adversary groups targeting organizations and employees. Adversary groups are regularly confused with their initial operation or campaign. MISP
- [clusters/tools.json](clusters/tools.json) - threat-actor-tools is an enumeration of tools used by adversaries. The list includes malware but also common software regularly used by the adversaries. MISP

# Available Vocabularies

## Common

- [vocabularies/common/certainty-level.json](vocabularies/common/certainty-level.json) - Certainty level of an associated element or cluster.

## Threat Actor

- [vocabularies/threat-actor/intended-effect-vocabulary.json](vocabularies/threat-actor/intended-effect.json) - The IntendedEffectVocab is the default STIX vocabulary for expressing the intended effect of a threat actor. STIX 1.2.1
- [vocabularies/threat-actor/motivation-vocabulary.json](vocabularies/threat-actor/motivation.json) - The MotivationVocab is the default STIX vocabulary for expressing the motivation of a threat actor. STIX 1.2.1
- [vocabularies/threat-actor/planning-and-operational-support-vocabulary.json](vocabularies/threat-actor/planning-and-operational-support.json) - The PlanningAndOperationalSupportVocab is the default STIX vocabulary for expressing the planning and operational support functions available to a threat actor.
- [vocabularies/threat-actor/sophistication.json](vocabularies/threat-actor/sophistication.json) - The ThreatActorSophisticationVocab enumeration is used to define the default STIX vocabulary for expressing the subjective level of sophistication of a threat actor.
- [vocabularies/threat-actor/type.json](vocabularies/threat-actor/type.json) - The ThreatActorTypeVocab enumeration is used to define the default STIX vocabulary for expressing the subjective type of a threat actor.

## How to contribute?

Fork the project, update or create elements or clusters and make a pull-request.

We recommend to validate the JSON file using [jq](https://stedolan.github.io/jq/) before doing a pull-request.

## License

MISP galaxy is licensed under [CC0 1.0 Universal (CC0 1.0)](https://creativecommons.org/publicdomain/zero/1.0/) -  Public Domain Dedication.
