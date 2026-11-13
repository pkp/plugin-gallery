<!--
Thank you for contributing to the Plugin Gallery! Before you submit, review the
release guide: https://docs.pkp.sfu.ca/dev/plugin-guide/en/release

PKP reviews every plugin and release before it is listed. New plugins and large
changes take longer to review, so please be patient and do not open duplicate
pull requests.

Plugins must be secure, follow PKP's coding conventions
(https://docs.pkp.sfu.ca/dev/documentation/en/), support translation, and be
transparent about what they do with users' data.

This template is required. Fill in every section unless it says otherwise, and
check every box in the checklist.

To check a box, replace [ ] with [x], or click the box after you create the
pull request. Do not check a box unless it is true.

Pull requests that do not complete this template, or do not answer it
truthfully, may be closed without review. A plugin that is later found to have
security issues, or that does not behave as described here, may be removed.
-->

## Plugin

- **Plugin name:**
- **Source code repository:**
- **Organizational affiliation (if any):**

**Type of change** (check one):

- [ ] New plugin
- [ ] New release of a plugin
- [ ] Compatibility update or correction to an existing entry

## About the plugin

<!-- New plugins only. What does the plugin do, and who is it for? If a plugin in the gallery or a feature of the application already does something similar, how is this one different? If you can, add screenshots or a short video of the plugin in use. -->

## Releases

<!--
For each release: the version, the application versions you tested it on, and
what changed since the last listed release. For example:

- 1.1.0.0 for OJS and OPS 3.5. Tested on OJS 3.5.0-5 and OPS 3.5.0-5. Adds
  compatibility with 3.5 and fixes the settings form not saving.
- 1.0.1.0 for OJS 3.4. Tested on OJS 3.4.0-10. Fixes the settings form not saving.
-->

## External services and data

Does the plugin send data to, or receive data from, any service outside the installation? (check one)

- [ ] No
- [ ] Yes. Describe the service, what data is sent, and when:

Does the plugin require an account, subscription or payment with a third party? (check one)

- [ ] No
- [ ] Yes. Describe the service, what is required, and any costs:

## AI use

Did you use AI tools to write the plugin code or this pull request? See [PKP's policy on AI contributions](https://pkp.sfu.ca/pkp-policy-ai/). (check one)

- [ ] No
- [ ] Yes. Describe how, and how you reviewed and tested the result:

## Checklist

- [ ] The plugin has a `LICENSE` file with a GPL-compatible open-source license (e.g. GPL, MIT, BSD, Apache 2.0), and its source code is public.
- [ ] The release package contains a single directory named after the plugin's `product`, with no tests, demos or development dependencies.
- [ ] The `<release>` in the package's `version.xml` matches the `version` in `plugins.xml`.
- [ ] The README describes what the plugin does, its requirements, how to configure it, and any data it sends outside the installation.
- [ ] I have considered security best practices, such as checking the user's role and access to the objects they request, escaping template output, using CSRF tokens, and preventing SQL injection.
- [ ] The repository has a private way to report security issues, such as [GitHub's private vulnerability reporting](https://docs.github.com/en/code-security/how-tos/report-and-fix-vulnerabilities/configure-vulnerability-reporting/configure-for-a-repository).
- [ ] I will respond to review comments myself, and will not post AI-generated responses or fixes without reviewing and testing them.

## Anything else reviewers should know (optional)
