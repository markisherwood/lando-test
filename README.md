# My Project

A brief description of My Project.

## Using This Template

Remove this section after initial setup!

Search for and replace the following placeholders within this file:

| Placeholder | Example |
| --- | --- |
| `#LOCAL_DEV_SITE_ALIAS` | `@example.local` |
| `#LOCAL_DEV_URL` | http://local.example.com/ |

## Getting Started

This project is based on BLT, an open-source project template and tool that enables building, testing, and deploying Drupal installations following Acquia Professional Services best practices. While this is one of many methodologies, it is our recommended methodology.

1. Review the [Required / Recommended Skills](http://blt.readthedocs.io/en/latest/readme/skills) for working with a BLT project.
2. Ensure that your computer meets the minimum installation requirements (and then install the required applications). See the [System Requirements](http://blt.readthedocs.io/en/latest/INSTALL/#system-requirements).
3. Fork the project repository in GitHub.
4. Setup a SSH key that can be used for GitHub and the Acquia Cloud (you CAN use the same key).
    1. [Setup GitHub SSH Keys](https://help.github.com/articles/adding-a-new-ssh-key-to-your-github-account/)
5. Clone your forked repository. By default, Git names this "origin" on your local.
    ```
    $ git clone git@github.com:<account>/#lando-test.git
6. To ensure that upstream changes to the parent repository may be tracked, add the upstream locally as well.
    ```
    $ git remote add upstream git@github.com:markisherwood/lando-test.git
    ```
7. Setup local environment.
    Lando is used as the local development environment. For instructions on settings up Lando, [read the documentation](https://docs.devwithlando.io/installation/installing.html).

    Once installed, the following command can be used to start the server.
    ```
    $ lando start
    ```

    Lando will install composer dependencies and setup the initial install.

9. Access the site and do necessary work at #LOCAL_DEV_URL by running this:
    ```
    $ lando drush uli
    ```

Additional [BLT documentation](http://blt.readthedocs.io) may be useful. You may also access a list of BLT commands by running this:
```
$ blt
```

Note the following properties of this project:
* Primary development branch: develop
* Local environment: #LOCAL_DEV_SITE_ALIAS
* Local site URL: https://mylandoapp.lndo.site

## Working With a BLT Project

BLT projects are designed to install software development best practices (including git workflows).

Our BLT Developer documentation includes an [example workflow](http://blt.readthedocs.io/en/latest/readme/dev-workflow/#workflow-example-local-development).

### Important Configuration Files

BLT uses a number of configuration (`.yml` or `.json`) files to define and customize behaviors. Some examples of these are:

* `blt/blt.yml` (formerly blt/project.yml prior to BLT 9.x)
* `blt/local.blt.yml`
* `box/config.yml` (if using Drupal VM)
* `drush/sites` (contains Drush aliases for this project)
* `composer.json` (includes required components, including Drupal Modules, for this project)

## Resources

* GitHub - https://github.com/markisherwood/lando-test
