# Kubernetes Config Selector
This script allows you to select a Kubernetes configuration file from a specified directory and set it as the current configuration by copying it to ~/.kube/config.

## Installation
Clone the Repository:

```sh
git clone <repository-url>
cd <repository-directory>
```
Make the Script Executable:

```sh
chmod +x chkube
```
## Usage

### Ensure Config Directory Exists:

Make sure you have a directory containing your Kubernetes configuration files at ~/.kube/configs. If this directory does not exist, create it and add your configuration files.

```sh
mkdir -p ~/.kube/configs
```

Execute the script to select and set the desired Kubernetes configuration file:

```sh
./chkube
```

The script will display a list of available configuration files. Choose the desired configuration by entering the corresponding number. The selected configuration file will be copied to ~/.kube/config, replacing the current configuration.

### Example
Assuming you have the following configuration files in ~/.kube/configs:

```sh
~/.kube/configs
├── config-cluster1
├── config-cluster2
└── config-cluster3

```
Running the script will display:

```sh
Select the configuration file you want to use:
1) config-cluster1
2) config-cluster2
3) config-cluster3
#?
```

Enter the number corresponding to the configuration you want to use, and the script will set it as your current Kubernetes configuration.

