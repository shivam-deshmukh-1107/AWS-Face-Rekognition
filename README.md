# Face Recognition Service with AWS Rekognition and Serverless Backend

An efficient Face Recognition Service built using AWS services. Upload images to an S3 bucket, trigger a Lambda function for analysis, create face prints stored in DynamoDB, and perform recognition to identify individuals.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- - [Face Upload and Processing](#face-upload-and-processing)
  - [Face Recognition](#face-recognition)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)
  - [Uploading Faces](#uploading-faces)
  - [Recognizing Faces](#recognizing-faces)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

Welcome to the Amazon S3 Face Recognition Service. This project showcases an end-to-end facial recognition system utilizing AWS S3, Lambda, and DynamoDB. Easily upload images, analyze them, create face prints, and perform recognition.

![10](https://github.com/shivamdeshmukh/Amazon_Face_Rekognition/assets/72214326/55dbecd9-db2b-4836-a7af-a86668ee90fa)

## Features

### Face Upload and Processing

- **Image Upload**: Upload images of individuals to an S3 bucket with associated metadata containing their names.
- **Lambda Trigger**: A Lambda function is triggered upon image upload, generating face prints for each image and storing them in DynamoDB.

### Face Recognition

- **Recognition**: Submit an image to the system for recognition.
- **Face Print Generation**: Analyze the image and generate a face print.
- **Database Lookup**: Search the DynamoDB database for matching face prints.
- **Result**: If a match is found, return the corresponding name; otherwise, indicate "person not detected".

## Getting Started

### Prerequisites

1. An AWS account.
2. AWS CLI installed and configured with your credentials.

### Installation

Clone the repository and install the required dependencies.

```bash
$ git clone https://github.com/your-username/s3-face-recognition.git
$ cd s3-face-recognition
$ pip install -r requirements.txt

