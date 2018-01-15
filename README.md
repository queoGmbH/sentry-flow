# [PunktDe.Sentry.Flow](https://github.com/punktDe/sentry-flow)

This is a Sentry client package for the Flow framework.

It's based on [Networkteam.SentryClient](https://github.com/networkteam/Networkteam.SentryClient).

Have a look at https://sentry.io for more information about Sentry.

## Installation

    $ composer require punktde/sentry-flow

## Configuration

Add the following to your `Settings.yaml` and replace the `dsn` setting with your project DSN (API Keys in your Sentry project):

```
PunktDe:
  Sentry:
    Flow:
      dsn: 'https://public_key:secret_key@your-sentry-server.com/project-id'
```

## Usage

Sentry will log all exceptions that have the rendering option `logException` enabled. This can be enabled or disabled
by status code or exception class according to the Flow configuration.
