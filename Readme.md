# Pochopedia Content

This repository contains the Pochopedia database.

## Database

The database files are split into three types:

* documents
* schemas
* templates

Document (or data) files (directory `data`) contain single database entries.
Each document has a schema (directory `schema`) that describes properties of the documents' keys.
For rendering the documents to HTML, templates (directory `template`) are used as determined by the schema.
Documents and schemas are [YAML](http://www.yaml.org/) files, templates are written in [Djula](http://mmontone.github.io/djula/).
Schemas support inheritance (one schema can "include" keys of other schemas) and templates are usually based on `template/main.tmpl`.

To get an impression of how the system works, have a look at the EG files ([`data/eg/`](data/eg), `schema/{`[`piece`](schema/piece.yaml),[`choral`](schema/choral.yaml),[`serial`](schema/serial.yaml),[`eg-choral`](schema/eg-choral.yaml),[`eg-choral-redirect`](schema/eg-choral-redirect.yaml)}`.yaml`, [`template/eg-choral.tmpl`](template/eg-choral.tmpl)) and the person files ([`data/persons/`](data/persons), [`schema/person.yaml`](schema/person.yaml), [`template/person.tmpl`](template/person.tmpl)).

## Contributing

You can contribute as usual using pull requests and issues. Feature branches for larger collections are appreciated.

More information to come.
