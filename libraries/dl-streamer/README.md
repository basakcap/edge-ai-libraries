# Intel® Deep Learning Streamer (Intel® DL Streamer) Pipeline Framework

## Overview
<div align="center"><img src="intro.gif" width=900/></div>

[Intel® Deep Learning Streamer](https://dlstreamer.github.io) (**Intel® DL Streamer**) Pipeline Framework is an open-source streaming media analytics framework, based on [GStreamer*](https://gstreamer.freedesktop.org) multimedia framework, for creating complex media analytics pipelines for the Cloud or at the Edge.

**Media analytics** is the analysis of audio & video streams to detect, classify, track, identify and count objects, events and people. The analyzed results can be used to take actions, coordinate events, identify patterns and gain insights across multiple domains: retail store and events facilities analytics, warehouse and parking management, industrial inspection, safety and regulatory compliance, security monitoring, and many other.

## Backend libraries
Intel® DL Streamer Pipeline Framework is optimized for performance and functional interoperability between GStreamer* plugins built on various backend libraries
* Inference plugins use [OpenVINO™ inference engine](https://docs.openvino.ai) optimized for Intel CPU, GPU and VPU platforms
* Video decode and encode plugins utilize [GPU-acceleration based on VA-API](https://github.com/GStreamer/gstreamer-vaapi)
* Image processing plugins based on [OpenCV](https://opencv.org/) and [DPC++](https://www.intel.com/content/www/us/en/develop/documentation/oneapi-programming-guide/top/oneapi-programming-model/data-parallel-c-dpc.html)
* Hundreds other [GStreamer* plugins](https://gstreamer.freedesktop.org/documentation/plugins_doc.html) built on various open-source libraries for media input and output, muxing and demuxing, decode and encode

[This page](https://dlstreamer.github.io/elements/elements.html) contains a list of elements provided in this repository.

## Prerequisites
Please refer to [System Requirements](https://dlstreamer.github.io/get_started/system_requirements.html) for details.

## Installation
Please refer to [Install Guide](https://dlstreamer.github.io/get_started/install/install_guide_ubuntu.html) for installation options
1. [Install APT packages](https://dlstreamer.github.io/get_started/install/install_guide_ubuntu.html#option-1-install-intel-dl-streamer-pipeline-framework-from-debian-packages-using-apt-repository)
2. [Run Docker image](https://dlstreamer.github.io/get_started/install/install_guide_ubuntu.html#option-2-install-docker-image-from-docker-hub-and-run-it)
3. [Compile from source code](https://dlstreamer.github.io/dev_guide/advanced_install/advanced_install_guide_compilation.html)
4. [Build Docker image from source code](https://dlstreamer.github.io/dev_guide/advanced_install/advanced_build_docker_image.html)

To see the full list of installed components check the [dockerfile content for Ubuntu24](https://raw.githubusercontent.com/open-edge-platform/edge-ai-libraries/refs/heads/main/libraries/dl-streamer/docker/dlstreamer_dev_ubuntu24.Dockerfile)

## Samples
[Samples](https://github.com/open-edge-platform/edge-ai-libraries/tree/main/libraries/dl-streamer/samples) available for C/C++ and Python programming, and as gst-launch command lines and scripts. 

## NN models
Intel® DL Streamer supports NN models in OpenVINO™ IR and ONNX* formats.
List of [supported models](<https://dlstreamer.github.io/supported_models.html>) which include LVM, object detection, object classification, human pose detection, sound classification, semantic segmentation, and other use cases on SSD, MobileNet, YOLO, Tiny YOLO, EfficientDet, ResNet, FasterRCNN and other backbones also pre-trained with [Intel® Geti™ Software](<https://www.intel.com/content/www/us/en/developer/tools/tiber/edge-platform/model-builder.html>)

## Reporting Bugs and Feature Requests
Report bugs and requests [on the issues page](https://github.com/open-edge-platform/edge-ai-libraries/issues)

## Other Useful Links
* [Get Started](https://dlstreamer.github.io/get_started/get_started_index.html)
* [Developer Guide](https://dlstreamer.github.io/dev_guide/dev_guide_index.html)
* [API Reference](https://dlstreamer.github.io/api_ref/api_reference.html)

---
\* Other names and brands may be claimed as the property of others.
