# GCP with Go monitoring implementation example

You can read more about GCP metrics and monitoring [here](https://cloud.google.com/monitoring/docs/reference/libraries#client-libraries-install-go)
## Overview

This Go application is tailored for monitoring the queue size in a video processing service. It employs OpenCensus for metrics collection and integrates with Google Cloud's Stackdriver for exporting these metrics, offering real-time insights into the processing load.

## Features

- **Real-time Queue Monitoring**: Tracks the queue length, providing a snapshot of the current workload.
- **Stackdriver Exporting**: Metrics are seamlessly exported to Stackdriver, facilitating comprehensive monitoring and alerting.
- **Environment-Based Configuration**: Utilizes environment variables for configuration, ensuring adaptability across various deployment environments.

## How It Works

The application simulates queue size checks for a hypothetical video processing service. It generates a random number between 1 and 100 every second to represent the queue size, mimicking a real-world scenario. These metrics are then exported to Stackdriver for analysis.

## Getting Started

### Prerequisites

- Go (latest stable version recommended)
- Access to Google Cloud Stackdriver

### Installation

1. Clone the repository to your local machine.
2. Install the required Go dependencies.

### Configuration

Configure the application using the following environment variables:

- `MY_PROJECT_ID` - Your Google Cloud Project ID.
- `MY_GCE_INSTANCE_ID` - The Compute Engine instance ID.
- `MY_GCE_INSTANCE_ZONE` - The zone of your Compute Engine instance.

## Usage

Execute the application by running `go run main.go`. This will initiate the queue size monitoring and begin exporting metrics to Stackdriver.

## Contributing

Welcome contributions that improve functionality or efficiency.
