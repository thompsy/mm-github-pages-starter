---
title: Thesis
description: "A Phd thesis about LTE networks"
tags: [research, phd]
share: false
permalink: /projects/jLTE-Simulator/
---

You can now download the final post-examination revision of my thesis,
titled [**Self-Organisation in LTE Networks: An
Investigation**](/self-organisation-in-lte-networks-final.pdf).

## Software

In the interests of repeatable research the software developed as part
of this thesis has been made available. Details about the software
components can be found below. Each of the components can be
downloaded from [github](http://github.com/thompsy/jLTE-Simulator).

### jLTE-Simulator

The jLTE-Simulator is an LTE network simulator designed and
implemented as part of this research. It is a physical layer simulator
tailored to the investigation of different schedulers on the
performance of the network.

### jLTE-EvolutionaryAlgorithm

The jLTE-EvolutionaryAlgorithm is an evolutionary algorithm
designed to be used in conjunction with the jLTE-Simulator. The
simulator is used as a fitness function to evolve parameter values for
new schedulers.

### jLTE-Experiments

The jLTE-Experiments project is an experiment framework built on the
jLTE-Simulator and jLTE-EvolutionaryAlgorithm projects. It contains
all the code required to run the experiments reported as part of my
thesis. The primary purpose of this project is to allow easy running
of experiments across a cluster of machines. Since each of the
experiments may run for a significant period of time, parallelising
the process across multiple hosts is a simple way to speed up the
process.


## Thesis Abstract
Mobile telecommunications networks based on LTE technology
promise faster throughput to their users. LTE networks are
however susceptible to a phenomenon known as inter-cell interference
which can greatly reduce the throughput of the network causing
unacceptable degradation of performance for cell edge users.

A number of approaches to mitigating or minimising inter-cell
interference have been presented in the literature such as
randomisation, cancellation and coordination. The possibility of
coordination between network nodes in an LTE network is made
possible through the introduction of the X2 network link.

This thesis explores approaches to reducing the effect of inter-cell
interference on the throughput of LTE networks by using the X2 link to
coordinate the scheduling of radio resources. Three approaches to the
reduction of inter-cell interference were developed. Localised
organisation is a centralised scheme in which a scheduler is optimised
by a GA to reduce interference. Networked organisation makes use of
the X2 communications link to enable the network nodes to exchange
scheduling information in a way that lowers the level of interference
across the whole network. Finally a more distributed and
de-centralised approach is taken in which each of the network nodes
optimises its own scheduling in coordination with its neighbours.

An LTE network simulator was built to allow for experimental
comparison between these techniques and a number of existing
approaches and to serve as a test bed for future algorithm
development. These approaches were found to significantly improve the
throughput of the cell edge users who were most affected by
interference. In particular the networked aspect of these approaches
yielded the best initial results showing clear improvement over the
existing state of the art. The distributed approach shows significant
promise given further development.
