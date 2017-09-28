# IBM Bluemix Quickstart Guide for N|Solid

This guide provides step-by-step instructions for deploying N|Solid on the IBM Cloud. N|Solid and N|Solid applications run on the IBM Cloud as Docker containers under Kubernetes. You can refer to the N|Solid Kubernetes quick start and production install information here: [https://github.com/nodesource/nsolid-kubernetes](https://github.com/nodesource/nsolid-kubernetes).

## Setup

The essential steps to prepare and setup N|Solid on the IBM Cloud are:

1. Register and create a Lite Kubernetes cluster using the 
[IBM Cloud Container Service](https://www.ibm.com/cloud-computing/bluemix/containers).

1. Install IBM Cloud Tools 
Linux/OSX install: 
```bash
curl -sL https://ibm.biz/idt-installer | bash
```
For Windows, see: [https://github.com/IBM-Bluemix/ibm-cloud-developer-tools](https://github.com/IBM-Bluemix/ibm-cloud-developer-tools).

1. Install N|Solid following either the [quickstart](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a2) or [production install](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a6) instructions. 
</li>
</eol>

## Installing Applications

- [Install a sample app for N|Solid with Kubernetes](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a5).

- [Configure Apps for N|Solid with Kubernetes](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a16).

- [Use IBM Cloud Developer Tools to create and deploy apps](https://developer.ibm.com/node/cloud/). This is the *fastest* way to create and deploy apps on the IBM Cloud.
