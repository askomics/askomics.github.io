---
layout: page
title: Documentation
permalink: /doc/
order: 3
---

## Manual installation

### Install dependencies

AskOmics needs python3.4 or higher, python3-venv, nodejs and npm.


### Download AskOmics

#### Stable version

Download the latest stable version of AskOmics [here](https://github.com/askomics/askomics/releases) or clone the AskOmics repository, and checkout the version manually

```bash
git clone https://github.com/askomics/askomics.git
cd askomics
git checkout 17.09
```


#### Development version

Clone the repository. The `master` branch contain the latest commits.

```bash
git clone https://github.com/askomics/askomics.git
```

### Download and install a triplestore

AskOmics can use the following triplestores:

- Virtuoso
- Allegrograph
- Corese
- RDF4j
- Fuseki


We advise you to use virtuoso.


### Run AskOmics

Run askomics using the `startAskomics.sh` script. This script will install all python dependencies into a virtual environment, and install all npm dependencies in the askomics directory.

The script take some options:

```bash
./startAskomics.sh -t <triplestore> -d <deployment_mode>
```

With \<triplestore\>, the used triplesore, and \<deployment mode\>: dev or prod. default is prod.


## Installation with docker-compose

### Dependencies

You will need docker and docker-compose. Installation instruction are [here](https://docs.docker.com/engine/installation/)

### Installation

Clone the askomics-docker-compose repository

```bash
git clone https://github.com/askomics/askomics-docker-compose.git
```


The askomics-docker-compose directory contain subdirectories. Choose one in function of what you need and run the command `docker-compose up`.

For example, for askomics + virtuoso + nginx + postfix, run

```bash
cd askomics-docker-compose/virtuoso
docker-compose up
```

AskOmics is now available at [http://localhost/askomics](http://localhost/askomics)
