# Scale Node.js with N|Solid and Kubernetes on IBM Bluemix Container Service

IBM recently announced the availability of Kubernetes for the Bluemix Container Service on the IBM Cloud, adding to an impressive list of services, including Watson Cognitive, BlockChain, Financial, Weather, Cloud Foundry, and many more. 

The Bluemix Container Service provides many advantages for managing a containerized environment, including service discovery, load balancing and abstracting away hardware are just a few from a very long list of benefits.

We are going to look at how to setup a Kubernetes cluster using the Bluemix Container Service, and how to deploy N|Solid to that environment. 

IBM has been hard at work, and has recently released a new cli tool that makes working with the IBM Cloud really simple. We will walk through all the steps to get you up and running with N|Solid and Kubernetes on Bluemix.

## Make a Bluemix Account 

Get started for free by creating your IBM Cloud account [here](https://www.ibm.com/cloud-computing/bluemix/).

## Install IBM Cloud Tools 
    
Linux/OSX:
```bash
curl -sL https://ibm.biz/idt-installer | bash
```
For Windows, see: 
[https://github.com/IBM-Bluemix/ibm-cloud-developer-tools](https://github.com/IBM-Bluemix/ibm-cloud-developer-tools).

This installs the Bluemix (bx) CLI and other tools you'll need for working with containers and Kubernetes, like Docker, Helm, and the Kubernetes CLI, kubectl. Don't worry if you have any of these tools already installed, the Cloud Tools installer will detect and skip right over them.

## Logging into to Bluemix via the CLI 

Login into your Bluemix account using the following command: 

```bash
bx login -a api.ng.bluemix.net 
```
Answer the prompts for email and password to complete the login.

## Create a Kubernetes Cluster 

Using the CLI, simply issue the following command to create a free Kubernetes cluster to get started: 

```bash
bx cs cluster-create --name mycluster 
```

This creates a Kubernetes cluster under the _Lite_ plan, which is a free single VM Kubernetes setup.  You can upgrade to the _Standard_ plan to add additional worker VMs for production app deployments. 

For further information, read all about the [IBM Cloud Container Service](https://www.ibm.com/cloud-computing/bluemix/containers).

## Installing N|Solid into a Kubernetes Cluster

Now, you've got Bluemix entirely primed and ready to deploy N|Solid with Kuberenetes. For the next steps to deploy N|Solid to Kubernetes on the IBM Cloud, you can take a look at the [production installation instructions](https://github.com/nodesource/nsolid-kubernetes#a6) - be sure to set up [persistent storage on Bluemix](https://github.com/cvignola/nsolid-kubernetes#a30), as well.

For even more information about Node.js, Kubernetes, and the associated tools,you can check out our webinar on [Getting Started with Node.js, Docker, and Kubernetes](http://pages.nodesource.com/getting-started-with-node-js-docker-kubernetes-wb.html), you can learn more about Kubernetes and its place as a part of the Node.js DevOps Stack for Digital Transformation, and you can learn some easy tricks for [improving your Node.js Docker images](https://nodesource.com/blog/8-protips-to-start-killing-it-when-dockerizing-node-js) to make deploying with Kubernetes even easier.

## Wrapping Up

Deploying Node.js applications to the cloud is made secure, reliable and connected using NodeSource. We're glad you're interested in deploying N|Solid to Kubernetes on the IBM Cloud,. In addition to N|Solid, you can take the risk out of your reliance on third-party Node.js modules when working locally,testing your applications in staging, deploying production to Bluemix, and more with [NodeSource Certified Modules](https://nodesource.com/products/certified-modules).

----

This guide provides step-by-step instructions for deploying N|Solid on the IBM Cloud. N|Solid and N|Solid applications run on the IBM Cloud as Docker containers under Kubernetes. Additionall, you can refer to the N|Solid Kubernetes quick start and production install information here: [https://github.com/nodesource/nsolid-kubernetes](https://github.com/nodesource/nsolid-kubernetes).

## Setup

The essential steps to prepare and setup N|Solid on the IBM Cloud are:

1. Register and create a Kubernetes cluster using the 
[IBM Cloud Container Service](https://www.ibm.com/cloud-computing/bluemix/containers).

1. Install IBM Cloud Tools 
    
    Linux/OSX:
    ```bash
    curl -sL https://ibm.biz/idt-installer | bash
    ```
    For Windows, see: 
    [https://github.com/IBM-Bluemix/ibm-cloud-developer-tools](https://github.com/IBM-Bluemix/ibm-cloud-developer-tools).

1. Install N|Solid following either the [quickstart](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a2) or [production install](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a6) instructions. 

## Installing Applications

- [Install a sample app for N|Solid with Kubernetes](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a5).

- [Configure Apps for N|Solid with Kubernetes](https://github.com/nodesource/nsolid-kubernetes/blob/master/README.md/#a16).

- [Use IBM Cloud Developer Tools to create and deploy apps](https://developer.ibm.com/node/cloud/). This is the *fastest* way to create and deploy apps on the IBM Cloud.
