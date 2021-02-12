# FIWARE Step-by-Step Tutorials (NGSI-LD)

[![Documentation](https://nexus.lab.fiware.org/repository/raw/public/badges/chapters/documentation.svg)](https://ngsi-ld-tutorials.rtfd.io)
[![License: MIT](https://img.shields.io/github/license/fiware/tutorials.Step-by-Step.svg)](https://opensource.org/licenses/MIT)
[![Support badge](https://img.shields.io/badge/tag-fiware-orange.svg?logo=stackoverflow)](https://stackoverflow.com/questions/tagged/fiware)
[![Docker](https://img.shields.io/docker/pulls/fiware/tutorials.ngsi-ld.svg)](https://hub.docker.com/r/fiware/tutorials.ngsi-ld/)
[![NGSI LD](https://img.shields.io/badge/NGSI-LD-d6604d.svg)](https://www.etsi.org/deliver/etsi_gs/CIM/001_099/009/01.03.01_60/gs_cim009v010301p.pdf)
[![JSON LD](https://img.shields.io/badge/JSON--LD-1.1-f06f38.svg)](https://w3c.github.io/json-ld-syntax/)
[<img src="docs/img/logo.png" align="right" width="162">](https://www.fiware.org/)<br/>
[![Documentation](https://img.shields.io/readthedocs/ngsi-ld-tutorials.svg)](https://ngsi-ld-tutorials.rtfd.io)
[![CI](https://github.com/FIWARE/tutorials.NGSI-LD/workflows/CI/badge.svg)](https://github.com/FIWARE/tutorials.NGSI-LD/actions?query=workflow%3ACI)

This is a collection of tutorials for the FIWARE ecosystem designed for **NGSI-LD** developers. Each tutorial consists
of a series of exercises to demonstrate the correct use of individual FIWARE components and shows the flow of context
data within a simple Smart Solution either by connecting to a series of dummy IoT devices or manipulating the context
directly or programmatically.

| :books: <br>[Documentation](https://ngsi-ld-tutorials.rtfd.io/) | <img src="https://json-ld.org/favicon.ico" align="center" height="25"> [NGSI-LD<br>Data Models](https://fiware.github.io/tutorials.Step-by-Step/schema/) | <img src="https://assets.getpostman.com/common-share/postman-logo-stacked.svg" align="center" height="25"> [Postman<br>Collections](https://explore.postman.com/team/3mM5EY6ChBYp9D) |  [![Docker Hub](https://nexus.lab.fiware.org/repository/raw/public/badges/docker/fiware.svg)](https://hub.docker.com/u/fiware) <br> [![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/fiware)](https://artifacthub.io/packages/search?repo=fiware) |  <img src="https://fiware.github.io/catalogue/img/fiware-emoji.png" height="20px" width="20px"/><br/> [**developer.fiware.org**](https://www.fiware.org/developers/) |
| ----------------------------------------------------------- | ------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---|

## Install

To download the full set of tutorials, simply clone this repository:

```console
git clone https://github.com/FIWARE/tutorials.NGSI-LD.git
cd tutorials.NGSI-LD/
git submodule update --init --recursive
```

### Swagger <img src="https://static1.smartbear.co/swagger/media/assets/swagger_fav.png" align="left"  height="30" width="30" style="border-right-style:solid; border-right-width:10px; border-color:transparent; background: transparent">

The OpenAPI Specification (commonly known as Swagger) is an API description format for REST APIs. A Swaggger spec allows
you to describe an entire API (such as NGSI-LD itself) however in this tutorial we shall be concentrating on using
Swagger to define data models.

API specifications can be written in YAML or JSON. The format is easy to learn and readable to both humans and machines.
The complete OpenAPI Specification can be found on GitHub:
[OpenAPI 3.0 Specification](https://github.com/OAI/OpenAPI-Specification/blob/master/versions/3.0.2.md). This is
important since we will need a well defined structure to be able to generate `@context` files.

### Docker and Docker Compose <img src="https://www.docker.com/favicon.ico" align="left"  height="36" width="36">

Each tutorial runs all components using [Docker](https://www.docker.com). **Docker** is a container technology which
allows to different components isolated into their respective environments.

-   To install Docker on Windows follow the instructions [here](https://docs.docker.com/docker-for-windows/)
-   To install Docker on Mac follow the instructions [here](https://docs.docker.com/docker-for-mac/)
-   To install Docker on Linux follow the instructions [here](https://docs.docker.com/install/)

**Docker Compose** is a tool for defining and running multi-container Docker applications. A series of `*.yaml` files
are used configure the required services for the application. This means all container services can be brought up in a
single command. Docker Compose is installed by default as part of Docker for Windows and Docker for Mac, however Linux
users will need to follow the instructions found [here](https://docs.docker.com/compose/install/)

You can check your current **Docker** and **Docker Compose** versions using the following commands:

```console
docker-compose -v
docker version
```

Please ensure that you are using Docker version 18.03 or higher and Docker Compose 1.21 or higher and upgrade if
necessary.

### Postman <img src="https://www.postman.com/favicon-32x32.png" align="left"  height="32" width="32">

The tutorials which use HTTP requests supply a collection for use with the Postman utility. Postman is a testing
framework for REST APIs. The tool can be downloaded from [www.getpostman.com](www.getpostman.com). All the FIWARE
Postman collections can downloaded directly from the
[Postman API network](https://explore.postman.com/team/3mM5EY6ChBYp9D)

### Cygwin for Windows <img src="https://www.cygwin.com/favicon.ico" align="left"  height="30" width="30">

We will start up our services using a simple Bash script. Windows users should download [cygwin](http://www.cygwin.com/)
to provide a command-line functionality similar to a Linux distribution on Windows.

## Tutorials List

### Core Context Management: NGSI-LD Fundamentals

&nbsp; 101. [Understanding `@context`](https://github.com/FIWARE/tutorials.Understanding-At-Context)<br/> &nbsp; 102.
[Working with `@context`](https://github.com/FIWARE/tutorials.Getting-Started/tree/NGSI-LD)<br/> &nbsp; 103.
[CRUD Operations](https://github.com/FIWARE/tutorials.CRUD-Operations/tree/NGSI-LD)<br/> &nbsp; 104.
[Entity Relationships](https://github.com/FIWARE/tutorials.Entity-Relationships/tree/NGSI-LD)<br/>&nbsp; 106.
[Subscriptions](https://github.com/FIWARE/tutorials.Subscriptions/tree/NGSI-LD)<br/>

### Internet of Things, Robots and third-party systems

&nbsp; 201. [Introduction to IoT Sensors](https://github.com/FIWARE/tutorials.IoT-Sensors/tree/NGSI-LD)<br/> &nbsp; 202.
[Provisioning the Ultralight IoT Agent](https://github.com/FIWARE/tutorials.IoT-Agent/tree/NGSI-LD)<br/>

### Core Context Management: Manipulating Context Data and Persisting Historic Data

&nbsp; 304. [Querying Time Series Data](https://github.com/FIWARE/tutorials.Time-Series-Data/tree/NGSI-LD) (QuantumLeap)<br/>

## Usage

Most tutorials supply a `services` script to start the containers:

```console
cd <tutorial-name>
git checkout NGSI-LD
./services start
```

### Following the tutorial exercises via Postman

Each tutorial submodule contains one or more `docker-compose.yml` files, along with a Postman collection containing the
necessary HTTP requests: import the collection into Postman and follow the instructions.

### Following the tutorial exercises from the command-line

Each submodule contains full instructions in README which details the appropriate bash commands (cUrl and Docker
Compose) to run.

Full instructions can be found within the [documentation](https://ngsi-ld-tutorials.rtfd.io/)

---

## License

[MIT](LICENSE) © 2020-2021 FIWARE Foundation e.V.
