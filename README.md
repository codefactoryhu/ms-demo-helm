# ms-demo

## Description
A Helm project that packages ms-demo-spring-boot application with its dependencies.

## Prerequisites
- Helm
- Kubernetes cluster

## Installation

### Install from OCI registry
1. Login to Helm repository:
    ```shell
    helm registry login -u {github-user} ghcr.io
    ```

2. Install Helm chart
    ```shell
    helm install ms-demo oci://ghcr.io/codefactoryhu/ms-demo --version={version}
    ```

### Install from source
3. Clone the repository:
    ```shell
    git clone https://github.com/codefactoryhu/ms-demo-helm.git
    ```

4. Change into the project directory:
    ```shell
    cd ms-demo-helm
    ```

5. Install the dependencies:
    ```shell
    helm dependency update
    ```

6. Customize the configuration by modifying the `values.yaml` file.

7. Deploy the Helm chart:
    ```shell
    helm install ms-demo .
    ```
