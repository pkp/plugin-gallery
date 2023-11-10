[![Build Status](https://app.travis-ci.com/pkp/plugin-gallery.svg?branch=main)](https://travis-ci.org/pkp/plugin-gallery)

# Plugin Gallery

This repository contains PKP's Plugin Gallery XML file. The live version of the file is published on: [http://pkp.sfu.ca/ojs/xml/plugins.xml](http://pkp.sfu.ca/ojs/xml/plugins.xml). This is what presents a list of compatible plugins in OJS, OMP, and OPS for possible installation.

## Adding A New Plugin

If you'd like to add a new plugin or plugin release to the Plugin Gallery, you can use Github to propose changes here. They will be tested and if they are accepted they will be merged and become part of the Plugin Gallery.

To add a new plugin, or make a new release of an existing plugin:

- Fork this repository to your own Github account
- Edit the [XML file](./plugins.xml) in your fork to add a new `<plugin>` or `<release>` element (see [Get the Plugin into the Plugin Gallery](https://docs.pkp.sfu.ca/dev/plugin-guide/en/release#get-the-plugin-into-the-plugin-gallery))
- Open a Pull Request against this repository with the updated XML from your fork
- Once it passes the build and it is reviewed by the maintainers, it will be merged and become part of the Plugin Gallery.

## Checks run on the PRs

- The XML is valid according to the [schema](http://pkp.sfu.ca/ojs/xml/plugins.xsd)
- The release package URL exists on the specified URL and matches the MD5 sum.
- [Coming] Check the contents of the gzipped file
- [Coming] Run smoke and integration tests for the plugin release
