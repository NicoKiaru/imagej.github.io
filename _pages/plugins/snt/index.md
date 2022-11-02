---
name: SNT
title: SNT
description: The ImageJ framework for quantification of neuronal anatomy.
forum-tag: snt
categories: [Segmentation,Neuroanatomy]
tags: snt,reconstruction,tracing,arbor,neuron,morphometry,dendrite,axon,neuroanatomy
nav-links: true
nav-title: Overview
artifact: org.morphonets:SNT
icon: /media/icons/snt.png
update-site: Neuroanatomy
doi: 10.1038/s41592-021-01105-7
---

SNT[^1] is ImageJ's framework for tracing, visualization, quantitative analyses and modeling of neuronal morphology. For tracing, SNT supports modern multi-dimensional microscopy data, semi-automated and automated routines, and options for editing traces. For data analysis, SNT features advanced visualization tools, access to all major morphology databases, and support for whole-brain circuitry data.

{% capture text%}
**SNT is available through Fiji and is based on [several publications](/plugins/snt/faq#how-do-i-cite-snt). If you use it successfully for your research please be so kind as to cite our work!**
{% endcapture %}
{% include notice icon="info" content=text %}

## Overview

SNT is toolbox for tracing and analyzing neuronal morphologies imaged using light microscopy. It aims to be as complete as possible, while remaining efficient to use. It can be used as a desktop application, or a [scripting library](/plugins/snt/scripting). It supersedes the original [Simple Neurite Tracer](/plugins/snt/faq#what-is-the-difference-between-snt-and-simple-neurite-tracer) software, and aggregates other tools previously scattered across the Fiji ecosystem of plugins, including [Sholl](/plugins/sholl-analysis)[^2] and [Strahler](/plugins/strahler-analysis) plugins.

The [source repository](https://github.com/morphonets/SNT) contains more details about the project, including a list of [features](https://github.com/morphonets/SNT#features), and [implementation details](https://github.com/morphonets/SNT/blob/master/NOTES.md#notes)

{% include gallery align="fill" content=
"
/media/plugins/snt/snt-overview.png | Overview diagram
/media/plugins/snt/snt-4D-examples.png | Semi-automated tracing: Support for multi-channel and timelapse images
/media/plugins/snt/snt-auto-tracing-overview.png | Fully automated tracing of segmented images
/media/plugins/snt/simpleneuritetracer2.png | Scripted routines co-exist with graphical user interface operations
/media/plugins/snt/snt-script-example.png | [Scripting](/plugins/snt/scripting) in any of Fiji's supported languages
/media/plugins/snt/snt-notebook.png | Scripting in native python through [pyimagej](/scripting/pyimagej)
/media/plugins/snt/snt-montage-light.png | Quantitative and publication quality visualizations
/media/plugins/snt/snt-montage-dark.png | Data-rich 3D visualizations
/media/plugins/snt/snt-ferris-wheel.png | Routines to summarize data from projectomes and connectomics
"
%}

## Installation

SNT is currently distributed through [Fiji](/software/fiji)'s [Neuroanatomy update site](/update-sites/neuroanatomy). The first time you start SNT from Fiji's menu structure ({% include bc path='Plugins|Neuroanatomy|SNT'%}, you should be prompted for automatic subscription and download of required dependencies. If not:

1. Run the Fiji [Updater](/plugins/updater) ({% include bc path='Help|Update..'%}, the penultimate entry in the {% include bc path='Help|'%} menu)
2. Click *Manage update sites*
3. Select the *Neuroanatomy* checkbox
4. Click *Apply changes* and restart Fiji.

**Optional**: For [sciview](/plugins/sciview) and [Cx3D](/plugins/snt/modeling) functionality, you need to install [sciview](/plugins/sciview). See the [official sciview documentation](https://docs.scenery.graphics/sciview) for details.

## Documentation

SNT's documentation is extensive. Please use the navigation bar on top of the page to access the different sections, organized as follows:

| Section                                                         | Contents                                                                                                                                     |
| --------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| **[Manual](/plugins/snt/manual)**                               | SNT's user guide for tracing operations                                                                                                      |
| **[Walk-throughs](/plugins/snt/step-by-step-instructions)**     | Detailed step-by-step instructions for specific tasks                                                                                        |
| **[Screencasts](/plugins/snt/screencasts)**                     | Video tutorials. If you are using SNT for the first time you probably want to start here                                                     |
| **[Reconstruction Viewer](/plugins/snt/reconstruction-viewer)** | SNT's entry point for visualization of pre-existing data. If you are analyzing neuronal reconstructions you may want to start here           |
| **[Analysis](/plugins/snt/analysis)**                           | Overview of all analysis commands, accessible in either the tracing interface or [Reconstruction Viewer](/plugins/snt/reconstruction-viewer) |
| **[Scripting](/plugins/snt/scripting)**                         | Details on how to use SNT as a scripting library                                                                                             |

## References

[^1]: {% include citation id='plugins/snt' %}
[^2]: {% include citation id='plugins/sholl-analysis' %}
