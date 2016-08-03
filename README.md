# rackhd-obm-migration
Tool for migrating RackHD OBM settings from the Mongo nodes collection to the obms collection

# Migrating RackHD OBM Settings to 2.0 OBM Model


## Setup

    clone the GIST containing the OBM migration script
    cd to the cloned directory
    npm install

## Running the migration script

    mongodump
    mv dump dump.save
    node obmMigration.js

NOTE: All mongo databases are backed up into the ./dump directory on startup.
      Use mongorestore to restore the database from backup.

