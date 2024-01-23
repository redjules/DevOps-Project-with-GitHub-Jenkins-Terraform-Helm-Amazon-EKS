# DevOps Project with GitHub Jenkins Terraform Helm Amazon EKS

Architecture:

<img width="355" alt="Screenshot 2024-01-23 at 10 17 59" src="https://github.com/redjules/DevOps-Project-with-GitHub-Jenkins-Terraform-Helm-Amazon-EKS/assets/106017493/5beb232f-a9d5-4eae-b9bf-2d3ff803db6a">

# Installation:

# Jenkins:

- Download Jenkins:

Visit the Jenkins website and download the latest stable Jenkins WAR (Web Application Archive) file for macOS.

- Open Terminal:

You can use the Terminal application on your Mac for the installation process.

- Run Jenkins:

Navigate to the directory where you downloaded the Jenkins WAR file.
Run the command java -jar jenkins.war to start Jenkins.
This will start Jenkins on its default port, which is 8080.

- Access Jenkins:

Open a web browser and go to http://localhost:8080.
The first time you access this page, Jenkins will ask you to unlock it using an administrator password.
Retrieve the password by following the instructions on the page. Typically, it involves opening a file in your home directory.

- Complete Setup:

Once you've unlocked Jenkins, you'll be guided through the initial setup process.
You can install suggested plugins or choose specific ones based on your needs.
After the plugins are installed, you will be prompted to create an admin user.
Configure Jenkins:

After setting up, you can configure Jenkins according to your project requirements. This may include setting up build jobs, configuring plugins, and adjusting system settings.

# Terraform:

Install Homebrew
If you don't already have Homebrew installed, follow these steps:

Open Terminal.
Run the following command:
bash
Copy code
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
Follow the on-screen instructions to complete the installation.

Install Terraform
Once Homebrew is installed, you can install Terraform:

Open Terminal.
Run the following command to install Terraform:
bash
Copy code
brew install terraform
Wait for the installation to complete.


To install Terraform on a Mac using Homebrew, you can follow these instructions written in Markdown format. Markdown is a lightweight markup language with plain-text formatting syntax. Here's how you can document the installation process:

markdown
Copy code
# Installing Terraform on macOS

This guide provides instructions on how to install Terraform on a Mac using Homebrew.

## Prerequisites

Before installing Terraform, ensure you have the Command Line Tools for Xcode installed. These tools are required for Homebrew, the package manager used to install Terraform.

### Install Command Line Tools for Xcode

1. Open **Terminal**.
2. Run the following command:
   ```bash
   xcode-select --install
Follow the prompts to complete the installation.

- Install Homebrew

If you don't already have Homebrew installed, follow these steps:

Open Terminal.
Run the following command:
bash
Copy code
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
Follow the on-screen instructions to complete the installation.

- Install Terraform

Once Homebrew is installed, you can install Terraform:

Open Terminal.
Run the following command to install Terraform:
bash
Copy code
brew install terraform
Wait for the installation to complete.

- Verify Installation

To ensure Terraform is installed correctly:

Open Terminal.
Run the following command:
bash
Copy code
terraform -version
You should see the Terraform version number in the output, confirming the successful installation.

# Helm:

1. **Open Terminal**: 
   - You can find the Terminal application in your `/Applications/Utilities` folder or search for it using Spotlight.

2. **Update Homebrew**:
   - It's always a good practice to update Homebrew before installing new packages. Run the following command in the Terminal:
     ```bash
     brew update
     ```

3. **Install Helm**:
   - Once Homebrew is updated, install Helm by running:
     ```bash
     brew install helm
     ```

4. **Verify Installation**:
   - To confirm that Helm has been installed successfully, run:
     ```bash
     helm version
     ```
   - This command should return the installed version of Helm.

## Post-Installation Steps

- **Initialize Helm**: 
  - Depending on your Kubernetes setup, you might need to initialize Helm and install Tiller, the server-side component of Helm. *Note: With Helm 3 and later, Tiller is no longer required.*

- **Configure Helm**:
  - You may need to configure Helm to work with your Kubernetes cluster. Refer to the official Helm documentation for specific configuration steps.
