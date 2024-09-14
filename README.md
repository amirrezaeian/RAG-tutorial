# RAG-tutorial
We show how to build a conversational RAG system using OCI GenAI service, OCI OpenSearch service and LangChain framework.

## Prerequisites

Here we assume that you already have an Oracle Cloud Account, have access to OCI Generative AI Agents, and OCI OpenSearch. 
If not, you can visit the following product pages for information to get them set up:
<ul><li> Oracle Cloud account: https://signup.cloud.oracle.com/ </li>
<li> OCI Generative AI Agents: https://docs.oracle.com/en-us/iaas/Content/generative-ai-agents/home.htm </li>
<li> Getting started with OCI OpenSearch: https://docs.oracle.com/en-us/iaas/Content/search-opensearch/home.htm </li>
</ul>

### 1. Set up

Follow links below to generate a config file and a key pair in your ~/.oci directory
<ul><li> https://docs.oracle.com/en-us/iaas/Content/API/Concepts/sdkconfig.htm </li>
<li> https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm </li>
<li> https://docs.oracle.com/en-us/iaas/Content/API/SDKDocs/cliinstall.htm#configfile </li>
</ul>
After completion, you should have following 2 things in your ~/.oci directory 
<ul><li> A config file(where key file point to private key:key_file=~/.oci/oci_api_key.pem) </li>
<li> A key pair named oci_api_key.pem and oci_api_key_public.pem </li>
</ul>    

Now make sure you change the reference of key file in config file (where key file point to private key:key_file=/YOUR_DIR_TO_KEY_FILE/oci_api_key.pem)

### 2. Upload Public Key

Upload your oci_api_key_public.pem to console: https://docs.oracle.com/en-us/iaas/Content/API/Concepts/apisigningkey.htm#three


### 3. Make sure you have python installed on your machine
```
python --version
```
 
### 4. Install all dependencies:

We suggest you install dependencies in a virtual env to avoid conflicts on your system
```
python3 -m venv venv
. venv/bin/activate
pip install -U oci
pip install langchain_community
pip install langchain_core
pip install langchain
pip install pypdf
```

## Notebooks:

### Demo_RAG.ipynb

In this notebook we show how to build a conversational RAG system using OCI GenAI service, OCI OpenSearch service and LangChain framework. 
Please update the setup section of the notebook before running. 


### Contributors

Author: Amir Rezaeian

Last release: 12 Sep 2024

This project is open source. Please submit your contributions by forking this repository and submitting a pull request!  

### License

Copyright (c) 2024 Oracle and/or its affiliates.

Licensed under the Universal Permissive License (UPL), Version 1.0.

See [LICENSE](LICENSE) for more details.

ORACLE AND ITS AFFILIATES DO NOT PROVIDE ANY WARRANTY WHATSOEVER, EXPRESS OR IMPLIED, FOR ANY SOFTWARE, MATERIAL OR CONTENT OF ANY KIND CONTAINED OR PRODUCED WITHIN THIS REPOSITORY, AND IN PARTICULAR SPECIFICALLY DISCLAIM ANY AND ALL IMPLIED WARRANTIES OF TITLE, NON-INFRINGEMENT, MERCHANTABILITY, AND FITNESS FOR A PARTICULAR PURPOSE.  FURTHERMORE, ORACLE AND ITS AFFILIATES DO NOT REPRESENT THAT ANY CUSTOMARY SECURITY REVIEW HAS BEEN PERFORMED WITH RESPECT TO ANY SOFTWARE, MATERIAL OR CONTENT CONTAINED OR PRODUCED WITHIN THIS REPOSITORY. IN ADDITION, AND WITHOUT LIMITING THE FOREGOING, THIRD PARTIES MAY HAVE POSTED SOFTWARE, MATERIAL OR CONTENT TO THIS REPOSITORY WITHOUT ANY REVIEW. USE AT YOUR OWN RISK.
