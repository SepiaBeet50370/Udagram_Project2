# High Availability Infrastructure as Code

This repository contains Infrastructure as Code (IaC) scripts to deploy the necessary network infrastructure, server infrastructure, and jumpbox infrastructure for a dummy application, PhotoGram, on Amazon Web Services (AWS) using AWS CloudFormation.

## Table of Contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Introduction

PhotoGram is an Instagram clone that aims to replicate the functionality and features of the popular social media platform. This repository provides the necessary IaC scripts to automate the provisioning of the underlying infrastructure required to deploy the PhotoGram application on AWS.

The infrastructure deployment is achieved using AWS CloudFormation, a service that allows you to create and manage AWS resources using declarative templates. The IaC scripts provided in this repository are designed to be deployed on AWS CloudFormation to automate the creation of network resources, server resources, and a jumpbox instance.

## Prerequisites

Before running the IaC scripts, ensure that you have the following prerequisites:

- An AWS account with sufficient permissions to create and manage resources.
- The AWS Command Line Interface (CLI) installed and configured on your local machine.
- Basic knowledge of AWS services and CloudFormation concepts.
- Familiarity with shell scripting (Bash) for executing the provided deployment scripts.

## Installation

To get started, follow these steps:

1. Clone this repository to your local machine:



























### Project Title - Deploy a high-availability web app using CloudFormation
### How to run the Deploy the Infrastructure?
You can run the infrastructure scripts in two easy steps:
```bash
# Ensure that the AWS CLI is configured before runniing the command below
# Create the network infrastructure
# Check the region in the create.sh file
./create.sh Network Network.yml NetworkParams.json
# Create servers
# Change the AMI ID and key-pair name in the servers.yml
# Check the region in the create.sh file
./create.sh Servers Servers.yml ServersParams.json
# Create the jump box
./create.sh JumpBox Jumpbox.yml JumpboxParams.json

```
### Infrastructure Diagram
See JPEG file for the infrastructure diagram