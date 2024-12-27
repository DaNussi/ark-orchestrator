# Ark Orchestrator

Ark Orchestrator is a project that automatically creates an Ark cluster with all maps using Helm charts for Kubernetes deployment.

## Features

- Automatically sets up an Ark cluster
- Includes all official maps
- Easy to configure and deploy on Kubernetes

## Requirements

- Kubernetes cluster
- Helm

## Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/ark-orchestrator.git
    cd ark-orchestrator
    ```

2. Install the Helm chart:
    ```sh
    helm install ark-cluster ./helm-chart
    ```

## Configuration

You can configure the cluster settings in the `values.yaml` file within the Helm chart directory.

## Usage

Once the cluster is up and running, you can connect to it using the Ark client. The server details will be displayed in the Kubernetes logs.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request.

## License

This project is licensed under the MIT License.