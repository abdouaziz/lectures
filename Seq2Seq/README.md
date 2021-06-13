
## Table of contents


> * [Title / Repository Name](#title--repository-name)
>   * [Introduction / Synopsis](#about--synopsis)
>   * [Table of contents](#table-of-contents)
>   * [The Paper](#installation)
>   * [Usage](#usage)
>     * [Screenshots](#screenshots)
>     * [Features](#features)
>   * [Code](#code)
>     * [Content](#content)
>     * [Requirements](#requirements)
>     * [Limitations](#limitations)
>     * [Build](#build)
>     * [Deploy (how to install build product)](#deploy-how-to-install-build-product)
>   * [Resources (Documentation and other links)](#resources-documentation-and-other-links)
>   * [Contributing / Reporting issues](#contributing--reporting-issues)
>   * [License](#license)
>   * [About Nuxeo](#about-nuxeo)



# Sequence to Sequence Learning with Neural Networks

Deep Neural Networks are powerful models that have achieved excellent performance on difficult learning tasks. Although DNNs work well whenever large labeled training sets are available, they cannot be used to map sequences to sequences. In this [paper](https://arxiv.org/pdf/1409.3215.pdf), they present a general end-to-end approach to sequence learning that makes minimal assumptions on the sequence structure. 

## Introduction 


Deep Neural Networks are powerful models that have achieved excellent performance on difficult learning tasks , 
Despite their flexibility and power, DNNs can only be applied to problems whose inputs and targets can be sensibly encoded with vectors of fixed dimensionality. It is a significant limitation, since many important problems are best expressed with sequences whose lengths are not known a-priori.

For example, speech recognition and machine translation are sequential problems. Likewise, question answering can also be seen as mapping a sequence of words representing the question to a sequence of words representing the answer .

Sequences pose a challenge for DNNs because they require that the dimensionality of the inputs and
outputs is known and fixed




 


## The Paper

In this paper, we show that a straightforward application of the Long
Short-Term Memory (LSTM) architecture [16] can solve general sequence to sequence problems.
The idea is to use one LSTM to read the input sequence, one timestep at a time, to obtain large fixeddimensional vector representation, and then to use another LSTM to extract the output sequence
from that vector (fig. 1).

A useful property of the LSTM is that it learns to map an input sentence of variable length into
a fixed-dimensional vector representation. Given that translations tend to be paraphrases of the
source sentences, the translation objective encourages the LSTM to find sentence representations
that capture their meaning, as sentences with similar meanings are close to each other while different


<p align="center">
<img src="../Images/Images/fig1.jpg">
</p>

## Usage

### Screenshots

### Features

## Code

[![Build Status](https://qa.nuxeo.org/jenkins/buildStatus/icon?job=/nuxeo/addons_nuxeo-sample-project-master)](https://qa.nuxeo.org/jenkins/job/nuxeo/job/addons_nuxeo-sample-project-master/)

### Content

Description, sub-modules organization...

### Requirements

See [CORG/Compiling Nuxeo from sources](http://doc.nuxeo.com/x/xION)

Sample: <https://github.com/nuxeo/nuxeo/blob/master/nuxeo-distribution/README.md>

### Limitations

Sample: <https://github.com/nuxeo-archives/nuxeo-features/tree/master/nuxeo-elasticsearch>

### Build

    mvn clean install

Build options:

* ...

### Deploy (how to install build product)

Direct to MP package if any. Otherwise provide steps to deploy on Nuxeo Platform:

 > Copy the built artifacts into `$NUXEO_HOME/templates/custom/bundles/` and activate the `custom` template.

## Resources (Documentation and other links)

## Contributing / Reporting issues

Link to JIRA component (or project if there is no component for that project). Samples:

* [Link to component](https://jira.nuxeo.com/issues/?jql=project%20%3D%20NXP%20AND%20component%20%3D%20Elasticsearch%20AND%20Status%20!%3D%20%22Resolved%22%20ORDER%20BY%20updated%20DESC%2C%20priority%20DESC%2C%20created%20ASC)
* [Link to project](https://jira.nuxeo.com/secure/CreateIssue!default.jspa?project=NXP)

## License

[Apache License, Version 2.0](http://www.apache.org/licenses/LICENSE-2.0.html)

## About Nuxeo

Nuxeo Platform is an open source Content Services platform, written in Java. Data can be stored in both SQL & NoSQL databases.

The development of the Nuxeo Platform is mostly done by Nuxeo employees with an open development model.

The source code, documentation, roadmap, issue tracker, testing, benchmarks are all public.

Typically, Nuxeo users build different types of information management solutions for [document management](https://www.nuxeo.com/solutions/document-management/), [case management](https://www.nuxeo.com/solutions/case-management/), and [digital asset management](https://www.nuxeo.com/solutions/dam-digital-asset-management/), use cases. It uses schema-flexible metadata & content models that allows content to be repurposed to fulfill future use cases.

More information is available at [www.nuxeo.com](https://www.nuxeo.com).