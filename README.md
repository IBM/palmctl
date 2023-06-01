# palmctl

This is the command line interface tool of IBM Hybrid Cloud Mesh (Mesh). It is used to configure and manage the [Mesh product](https://www.ibm.com/products/hybrid-cloud-mesh).

You can subscribe to Mesh at [My IBM](https://myibm.ibm.com/). Once you have done that, visit [Mesh CLI Guide](https://www.ibm.com/docs/en/hybrid-cloud-mesh-eap?topic=cli-guide) for a brief overview of `palmctl`, along with its installation procedure and some examples.

## Downloading and Installing the CLI on Ubuntu

```
PALMCTL_FILE_NAME=palmctl-amd64.deb
curl -sSfLO https://github.com/IBM/palmctl/releases/latest/download/$PALMCTL_FILE_NAME
sudo apt install "$PWD/$PALMCTL_FILE_NAME"
```
{: codeblock}

## Downloading and Installing the CLI on RHEL

```
PALMCTL_FILE_NAME=palmctl-x86_64.rpm
curl -sSfLO https://github.com/IBM/palmctl/releases/latest/download/$PALMCTL_FILE_NAME
sudo rpm -i "$PWD/$PALMCTL_FILE_NAME"
```
{: codeblock}

## Downloading and Installing on Mac OSX amd64

```
PALMCTL_FILE_NAME=palmctl-amd64.tar.gz
curl -sSfLO https://github.com/IBM/palmctl/releases/latest/download/$PALMCTL_FILE_NAME
tar -xvf $PALMCTL_FILE_NAME
sudo ./palmctl/install.sh
source /usr/local/etc/bash_completion.d/bash_palmctl_completion
```
{: codeblock}

## Downloading and Installing on Mac OSX arm64

```
PALMCTL_FILE_NAME=palmctl-arm64.tar.gz
curl -sSfLO https://github.com/IBM/palmctl/releases/latest/download/$PALMCTL_FILE_NAME
tar -xvf $PALMCTL_FILE_NAME
sudo ./palmctl/install.sh
source /usr/local/etc/bash_completion.d/bash_palmctl_completion
```
{: codeblock}

**Mac OSX notes:**

- To enable auto-completion in the `zsh` or `fish` shells, see the output of the `sudo ./palmctl/install.sh` command.
- If you download the `palmctl` package using the browser, when you run `palmctl`, OSX will give you the error message `"palmctl" cannot be opened because the developer cannot be verified`. To enable it, open `System Settings`, go to the `Privacy & Security` tab, and scroll to the `Security` section. You will see `"palmctl" was blocked from use because it is not from an identified developer`. Click `Allow Anyway`. (The `palmctl` OSX package will be notarized in a future release.)

## Verifying the CLI installation:

```
palmctl --version
```
{: codeblock}
