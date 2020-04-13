# Rapid Digital Response kit

<p align="center">
<a href="https://console.platform.sh/projects/create-project?template=https://github.com/annex-digital/rapid-digital-response-kit.git@master">
    <img src="https://platform.sh/images/deploy/lg-blue.svg" alt="Deploy on Platform.sh" width="180px" />
</a>
</p>

The Rapid Digital Response kit is a quick start project for Australian Government teams dealing with the requirements of rapid project creation when responding to crisis. It was created by the team at Annex Digital in response to COVID-19.

## What can you use this for?

This project is especially designed for projects which require fast setup, compliance and security, and Australian Government branding (via the UI Kit), but which do not require heavy customisation.

## Getting Started

You can download and run Rapid wherever you like, however Rapid is designed as a 1-click install on Platform.sh.

## Stack

This project relies on or is designed for the following:

- Drupal 8
- PHP 7.2
- MariaDB 10.2
- Lando
- Visual Studio Code
- Platform.sh (and the Platform.sh CLI), though other hosting can also be used.

## Optional Drupal modules
### Sentry (via the Raven module)
Sentry.io tracks application bugs. The Raven module will automatically collect your Drupal logs and forward specific
types of warnings to Sentry. A Sentry account is required.

To automatically provide the Sentry DSN on Platform.sh, use the following to set a project variable:

```
$ platform variable:create --sensitive true --name env:sentry_dsn --value <your sentry dsn>
```

Setting this value in your top level environment will cascade it through child environments, giving you full error
reporting on all environments. To run it on your production branch only, use `--inheritable false`.

### ElasticSearch (via the ElasticSearch Connector module)


### Swiftmailer

Additionally, when running on Platform.sh:

- Nginx

## Alternatives

* [GovCMS](https://www.govcms.gov.au/)

## References

* [Drupal](https://www.drupal.org/)
* [Drupal on Platform.sh](https://docs.platform.sh/frameworks/drupal8.html)
* [PHP on Platform.sh](https://docs.platform.sh/languages/php.html)
