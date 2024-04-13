# Phylogenomics
In the world of Python programming and data science, Conda is a powerful tool for managing packages and environments. If you’re using Ubuntu and want to harness the full potential of Conda, this step-by-step guide will walk you through the installation process and help you create your own Conda environment. Let’s dive in!

Installing Conda:

Update Packages: First things first, make sure your system is up to date by running the following command in your terminal:

    sudo apt-get update

Install Curl: If you don’t already have Curl installed, you can do so by running:

    sudo apt-get install curl

Download Anaconda: Head over to the Anaconda website (https://www.anaconda.com/products/individual) and download the latest version. You can use the terminal to download it directly to your /tmp directory:

    cd /tmp
    curl -O https://repo.anaconda.com/archive/Anaconda3-2020.11-Linux-x86_64.sh

Run Anaconda Script: Execute the Anaconda script you just downloaded. By default, it will install Anaconda in your home directory under /home/<username>/anaconda3. Replace <username> with your actual username.

    bash Anaconda3–2020.11-Linux-x86_64.sh

Initialize Conda: After installation, initialize Conda by running:

    source ~/.bashrc

Check Conda Version: Verify that Conda is installed correctly by checking its version:

conda -V
You should see something like:

    conda 4.9.2

Updating Conda:

To keep your Conda installation up to date, periodically run these commands:

    conda update conda
    conda update anaconda

Creating a Conda Environment:

Now that you have Conda up and running, let’s create a Conda environment.
Create Environment: To create a new environment named ‘My_env1’ with Python 3, use the following command:

    conda create — name My_env1 python=3

Activate Environment: Once created, activate your new environment:

    conda activate My_env1

Deactivate Environment: To deactivate the environment when you’re done working in it, simply run:

    conda deactivate

Installing Packages: Installing packages in your Conda environment is a breeze. Use the following command, replacing <package-name> with the package you want to install and [=version] with the optional version you desire:

    conda install <package-name>[=version]

Conclusion: You’ve successfully installed Conda on your Ubuntu system and created your first Conda environment. With Conda, you can now manage packages and dependencies with ease, making your Python development and data science projects smoother and more efficient. Happy coding!
