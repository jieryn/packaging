# Branding Definition
Branding definition file has the following variables

* `RELEASELINE`: used only for OSS Jenkins releases. This variable selects one of the 4 release lines that we
  maintain (empty for mainline releases, "-rc" for RCs, "-stable" for LTS, and "-stable-rc" for LTS RCs.)
* `PRODUCTNAME`: Short human readable name of the product. Should be something like "Acme Foo Bar Zot".
  Used as the title of the product.
* `SUMMARY`: One line human readable description of what the product does.
* `ARTIFACTNAME`: Alpha-numeric lower-case (plus '-' and '_') only machine name of the product. Used as the stem of the file names.
* `CAMELARTIFACTNAME`: Alpha-numeric machine name of the product, but in CamelCase (such as FooBarZot.)
  By convention this name should not have '-' or '_'
* `VENDOR`: Short human readable name of the entity that generates the package.
* `PORT`: TCP/IP port that Jenkins will bind to out of the box.
* `MSI_PRODUCTCODE`: Windows installer uses UUID to identify which MSI files are of the same lineage.
  If two MSIs have the same UUID, one will overwrite another. So if you are to produce your own MSI,
  you need to use a different UUID.
* `OSX_IDPREFIX`: prefix of the various IDs in OS X. This follows the reverse domain name format.