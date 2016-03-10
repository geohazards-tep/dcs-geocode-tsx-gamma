## Developer Cloud Sandbox TerraSAR-X geocoding with GAMMA

The GAMMA SAR and Interferometry Software is a collection of programs that allows processing of SAR, interferometric SAR (InSAR) and differential interferometric SAR (DInSAR) data for airborne and spaceborne SAR systems. The software supports the entire processing from raw data to high level products such as digital elevation models, displacement maps,  point target analysis and landuse maps.

## Quick link
 
* [Getting Started](#getting-started)
* [Installation](#installation)
* [Submitting the workflow](#submit)
* [Community and Documentation](#community)
* [Authors](#authors)
* [Questions, bugs, and suggestions](#questions)
* [License](#license)

### <a name="getting-started"></a>Getting Started 

To run this application you will need a Developer Cloud Sandbox with GAMMA that can be either requested from:
* ESA [Geohazards Exploitation Platform](https://geohazards-tep.eo.esa.int) for GEP early adopters;

A Developer Cloud Sandbox provides Earth Sciences data access services, and helper tools for a user to implement, test and validate a scalable data processing application. It offers a dedicated virtual machine and a Cloud Computing environment.
The virtual machine runs in two different lifecycle modes: Sandbox mode and Cluster mode. 
Used in Sandbox mode (single virtual machine), it supports cluster simulation and user assistance functions in building the distributed application.
Used in Cluster mode (a set of master and slave nodes), it supports the deployment and execution of the application with the power of distributed computing for data processing over large datasets (leveraging the Hadoop Streaming MapReduce technology). 

### <a name="installation"></a>Installation

#### Pre-requisites

TBW

##### Using the releases

Log on the developer cloud sandbox. Download the rpm package from https://github.com/Terradue/dcs-stamps-ps/releases.
Install the dowanloaded package by running these commands in a shell:

```bash
sudo yum -y install dcs-geocode-tsx-gamma-<version>.x86_64.rpm
```

#### Using the development version

Log on the Developer Cloud Sandbox and run these commands in a shell:

```bash

git clone git@github.com:geohazards-tep/dcs-geocode-tsx-gamma.git
cd dcs-geocode-tsx-gamma
mvn install
```

### <a name="submit"></a>Submitting the workflow

Run this command in a shell:

```bash
ciop-run
```
Or invoke the Web Processing Service via the Sandbox dashboard or the [Geohazards Thematic Exploitation platform](https://geohazards-tep.eo.esa.int) providing a stack of TerraSAR-X product URLs.

### <a name="community"></a>Community and Documentation

To learn more and find information go to 

* [Developer Cloud Sandbox](http://docs.terradue.com/developer) service 
* [GAMMA](http://www.gamma-rs.ch/gamma.html)
* [ESA Geohazards Exploitation Platform](https://geohazards-tep.eo.esa.int)

### <a name="authors"></a>Authors (alphabetically)

* Brito Fabrice
* Rossi Cesare

### <a name="questions"></a>Questions, bugs, and suggestions

Please file any bugs or questions as [issues](https://github.com/geohazards-tep/dcs-geocode-tsx-gamma/issues/new) or send in a pull request if you corrected any.

### <a name="license"></a>License

Copyright 2016 Terradue Srl

Licensed under the Apache License, Version 2.0: http://www.apache.org/licenses/LICENSE-2.0
