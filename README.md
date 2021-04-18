= OWL Standard document for PASS

The Web Ontology Lanague (OWL) is used to specify the structure of the subject-oriented modeling language PASS (Parallel Activity Specification Schema).

This repository contains the latest (development) version of the "Standard PASS Ont". See [/releases] for all releases.

You can find the documentation of this ontology in a separate repository: https://github.com/I2PM/PASS-Standard-Book-Tex-Project

== Development / releases

The version history / changelog is contained within the file itself as comment of the ontology.

To perform a new release, do the following steps:
* decide for a VERSION string, e.g. 1.2.3
* describe the changes in the version history comment of the ontology, mention both the current date and the VERSION
  * commit this change with the message "prepare vVERSION", tag it as "vVERSION" and push both the commit and the tag to this GitHub repository
* make a local copy of the file `standard_PASS_ont_dev.owl` and name it `standard_PASS_ont_v_VERSION.owl`
  * in that copy, update owl:versionIRI from "dev" to VERSION
* go to the release in this GitHub repository for "vVERSION"
  * copy the description of the current changes to the release description
  * upload your local file as an asset
  * publish the release
* update owl:priorVersion in `standard_PASS_ont_dev.owl` to the VERSION
  * commit & push this change with the message "prepare next development iteration"
