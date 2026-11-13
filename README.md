[![Build Status](https://github.com/pkp/plugin-gallery/actions/workflows/main.yml/badge.svg)](https://github.com/pkp/plugin-gallery/actions/workflows/main.yml)

# Plugin Gallery

This repository contains the Plugin Gallery for OJS, OMP and OPS. The Plugin Gallery lets site administrators install plugins from inside the application.

The gallery is a single XML file, [`plugins.xml`](./plugins.xml), that is validated against the schema in [`plugins.xsd`](./plugins.xsd). When changes are merged, the file is published at [https://pkp.sfu.ca/ojs/xml/plugins.xml](https://pkp.sfu.ca/ojs/xml/plugins.xml), where the applications read it. Each installation only shows the plugins whose releases are compatible with its version.

## Add or Update a Plugin

Review [Release a Plugin](https://docs.pkp.sfu.ca/dev/plugin-guide/en/release) in the Plugin Guide before you begin. It explains how to package your plugin and format its entry in `plugins.xml`.

1. Publish a release package (`.tar.gz`) of your plugin at a public, permanent URL, such as a GitHub release.
2. Fork this repository and create a branch from the latest `main`.
3. Edit `plugins.xml`. See [Get the Plugin into the Plugin Gallery](https://docs.pkp.sfu.ca/dev/plugin-guide/en/release#get-the-plugin-into-the-plugin-gallery) for an example entry and how to format each element. To add a release, add a new `<release>` element, and do not change or remove existing releases.
4. Open a pull request against `main` and fill in the pull request template. Check the "Files changed" tab to make sure that only your plugin's entry has changed.

If you publish a newer release while your pull request is waiting for review, update the pull request rather than opening a new one.

## Review

Every new plugin and release is reviewed by PKP before it is merged. A PKP team member will review the plugin's code, especially for security, the handling of users' data, and compatibility. Reviewers will comment on the pull request if anything needs to change.

Reviewers may use AI tools to help find issues. Every finding is checked by a reviewer before it is posted, and the decision to list a plugin is always made by a person.

When you respond to review comments, follow [PKP's policy on AI contributions](https://pkp.sfu.ca/pkp-policy-ai/): review and test any changes yourself, and do not post AI-generated responses or fixes without checking them.

Reviews are done by a small team. New plugins and large changes can take several weeks to review, so please be patient and do not open duplicate pull requests.

## Automated Checks

Every pull request runs automated checks, which must pass before it can be merged. They check that:

- `plugins.xml` is valid according to `plugins.xsd`.
- Each new release package can be downloaded from its URL and matches the `md5` in `plugins.xml`.

## Questions

If you have a question about the Plugin Gallery or plugin development, ask on the [PKP Community Forum](https://forum.pkp.sfu.ca/).
