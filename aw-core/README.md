aw-core
=======

Core library for AlantisWatch.


## Modules

 - `aw_core`, contains basic datatypes and utilities, such as the `Event` class, helpers for configuration and logging, as well as schemas for buckets, events, and exports.
 - `aw_datastore`, contains the datastore classes used by aw-server-python.
 - `aw_transform`, all event-transforms used in queries.
 - `aw_query`, the query-language used by ActivityWatch.


## How to install

To install the latest git version directly from github without cloning, run
`pip install git+https://github.com/atlantis-watch/aw-core.git`

To install from a cloned version, cd into the directory and run
`poetry install` to install inside an virtualenv. If you want to install it
system-wide it can be installed with `pip install .`, but that has the issue
that it might not get the exact version of the dependencies due to not reading
the poetry.lock file.

