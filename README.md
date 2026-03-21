# taxonpages-community-panels
Custom panels that were made by the community for [TaxonPages](https://github.com/SpeciesFileGroup/taxonpages).\
See them live at https://catalog.curculionoidea.org (Source repository: https://github.com/Curculionidae/taxa)

## Disclaimer
The panels that are currently here were coded using Claude Code. I guess the code can be written more elegantly, and the documentation may be weird (because it is AI-generated).

## How to install panels
Copy the folder of the panel into the /panels directory on the setup branch of your [TaxonPages](https://github.com/SpeciesFileGroup/taxonpages).\
As explained in the readme of the TaxonPages repository, you have to add the panel to the config/taxa-page.yml file to control their position:

```yaml
taxa_page:
  overview:
    panels:
      - - - panel:gallery
          - panel:type
          - panel:type-specimen
          - panel:nomenclature
          - panel:nomenclature-references

        - - panel:map
          - panel:descendants
          - panel:content
          - panel:statistics
          - panel:keys
          - panel:sounds

# An example of a new tab:

type_specimens:
   rank_group: ['SpeciesGroup']
   panels:
     - - - panel:specimen-records
```

## How to contribute
Fork this repository. Git clone your fork on your local system, copy a panel to your local clone of TaxonPages to start working. Using e.g. Claude (or Claude Code), it is not complicated to modify panels or create new ones. When vibe coding, make sure to provide enough context to the AI agent (API documentation for TaxonWorks, relevant files from the TaxonPages directory).\
To contribute back to this repository, go to the directory where you cloned your fork of this repository. Replace the folder of the panel you modified with your modified version. Use Git to commit your changes with a meaningful description, git push to your fork on Github. Now, you can open a pull request to contribute back to this repository.
