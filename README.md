# CmdfaceClient

This application is meant to provide a device-side wrapper for Cmdface tasks.
It is meant to:

- Sync new devices to Cmdface
- Unsync (destroy) devices you no longer want on Cmdface
- Generate `Facefile`s
- Setup and sync new commands
- Run commands as instructed by the external API

The client is designed to be secure. Only commands you explicitly whitelist
will be included on the Cmface web interface/API.

## Installation

## Setup

On the device that you want to sync, be sure to setup your organization unique
identifier.

```
export CMDFACE_ORGANIZATION_ID={your-id}
```

You can find your organization ID on the [Cmdface dashboard](https://cmdface.com/dashboard).

## Usage

Basic usage for the client is `cmdface {command} {options}`.

###### `diag`

Command ensures that you are able to connect to the Cmdface servers. It also
provides diagnostic information about the current environment.

###### `facefile`

Generates a blank Facefile scaffold.
