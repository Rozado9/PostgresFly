# PostgresFly
A streamlined tool for remotely installing PostgreSQL on Linux machines using a Windows interface. Fly through your setup with PostgresFly!

**PostgresFly** is an efficient tool designed for Windows users to remotely install various versions of PostgreSQL on Linux machines. Following the installation of PostgreSQL, PostgresFly provides a backup script to facilitate regular backups of your PostgreSQL database. With its user-friendly interface, PostgresFly allows for the installation of the desired PostgreSQL version on a Linux server with just a few inputs and a single click.


![Screenshot von PostgresFly](PostgresFly.png)


## Operating System:
- The tool is developed for Windows and facilitates the installation of various PostgreSQL versions on a Linux machine via a remote connection.

# Prerequisites

## User Permissions on the Linux Machine:
- The executing user must have `sudo` permissions.
- In `/etc/sudoers`, the entry `Username ALL=(ALL) NOPASSWD:ALL` should be present. Replace "Username" with the actual username.

## Directory Structure on the Linux Machine:
- A `pg-data` directory should be present in the root directory where PostgreSQL data will be stored.
  ```bash
  sudo mkdir /pg-data

## Required Software on Linux Machines:
- **SSH** for remote connection:
  ```bash
  sudo apt install openssh-server

- **PowerShell** for backup tasks using the provided script:
  ```bash
  sudo apt-get update
  sudo apt-get install -y wget apt-transport-https software-properties-common
  source /etc/os-release
  wget -q https://packages.microsoft.com/config/ubuntu/$VERSION_ID/packages-microsoft-prod.deb
  sudo dpkg -i packages-microsoft-prod.deb
  rm packages-microsoft-prod.deb
  sudo apt-get update
  sudo apt-get install -y powershell

## Starting the Application

1. Download and extract the `PostgresFly.zip` file from GitHub.
2. Navigate to the extracted folder.
3. Double-click on `PostgresFly.exe` to launch the program.


    

