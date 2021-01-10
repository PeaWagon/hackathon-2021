# Hello World using .NET and C&#35;

## Install .NET

Here are the [instructions](https://docs.microsoft.com/en-us/dotnet/core/install/linux-ubuntu#2004-) I followed to install .NET on Ubuntu 20.04.1 LTS.

1. Add Microsoft signing key and repository to apt (see details in `/etc/apt`).

    ```bash
    wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
    sudo dpkg -i packages-microsoft-prod.deb
    ```

2. Install .NET SDK (no runtime needed).

    ```bash
    sudo apt-get update; \
    sudo apt-get install -y apt-transport-https && \
    sudo apt-get update && \
    sudo apt-get install -y dotnet-sdk-5.0
    ```

## Generate the code

Made by following [this tutorial](https://dotnet.microsoft.com/learn/dotnet/hello-world-tutorial/intro).

To generate the code, use:

```bash
dotnet new console -o helloWorld
```

## Run the code

To run the project, `cd` into the `helloWorld` folder and enter:

```bash
dotnet run
```


