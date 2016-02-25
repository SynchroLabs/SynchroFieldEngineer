# SynchroFieldEngineer - Synchro FieldEngineer sample app

This app is intended to be installed into a [Synchro Server](https://synchro.io) environment using the [Synchro Command Line Interface](https://www.npmjs.com/package/synchro) tool.  

The Synchro FieldEngineer app was a quick and dirty prototype modelled after the Microsoft Azure Field Engineer sample app.  It is primarily good to illustrate how you would populate a Synchro ViewModel from an MSSQL database.

## Installing Synchro FieldEngineer

To install in your Synchro Server environment using the Synchro CLI:
```
$ synchro install https://github.com/SynchroLabs/SynchroFieldEngineer/archive/master.zip
```

Alternatively, you may use Git to install this app and keep it up to date.  To do that, you will want to clone SynchroFieldEngineer (this repo) into the `synchro-apps` directory in your Synchro installation, then install Synchro FieldEngineer into your configuration using the Synchro CLI:

```
$ synchro add SynchroFieldEngineer synchro-field-engineer
```

## Configuring Synchro FieldEngineer

The following configuration settings are required (they should point to an MSSQL database with an appropriate schema and intial data).

DB_USER
DB_PASSWORD
DB_SERVER
DB_NAME

## Updating Synchro FieldEngineer

If you installed this app using `synchro install`, then you may update it (getting the most recent version) at any time by doing:

```
$ synchro install -u synchro-field-engineer
```

Of course if you installed by cloning the repo, then you will use Git to update as appropriate.
