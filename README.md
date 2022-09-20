# ccd-ahm-2022
Contains my code and deck for [Cloud Community Days Ahmedabad 2022](https://gdg.community.dev/events/details/google-gdg-cloud-ahmedabad-presents-google-cloud-community-day-2022/): **Fantastic ML Deployments and How to Do Them with Vertex AI**. 

## Prerequisites

The notebooks provided in this repository use _paid_ Google Cloud Platform (GCP) services:

* [Vertex AI Workbench](https://www.youtube.com/watch?v=_Q1Nf-rgSiE)
* [Google Cloud Storage (GCS)](https://cloud.google.com/storage)
* [Vertex AI Prediction](https://cloud.google.com/vertex-ai/docs/predictions/getting-predictions)
* [Google Container Registry (GCR)](https://cloud.google.com/container-registry)

So, I assume you already have a billing-enabled GCP Project and you can:

* spin up Vertex AI Workbench instances
* create buckets on GCS
* push Docker images to GCR

## Notebooks

The notebooks are in `notebooks` directory. Below is a brief description of each notebook:

* `resnet-export.ipynb` shows how to export a TensorFlow model (image recognition) compatible with
off-the-shelf Vertex AI deployment.
* `onnx-conversion.ipynb` shows how to optimized the TensorFlow model with ONNX and compares the latency
of the both the models (TensorFlow and ONNX).
* `custom-onnx-deployment.ipynb` shows how to deploy the ONNX model to Vertex AI using custom prediction
routes.

## Slides

TBA

## Acknowledgements

Thanks to the ML Developer Programs team at Google for providing GCP credit support.
