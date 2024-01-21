# Snort-3-Easy-Script
This bash script automates the installation and basic configuration of Snort, a powerful Network Intrusion Detection System (NIDS), on your Linux system.


# Snort 3 Easy Script


**Automated Installation and Configuration of Snort 3**

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
  - [1. Clone the Repository](#1-clone-the-repository)
  - [2. Navigate to the Script Directory](#2-navigate-to-the-script-directory)
  - [3. Run the Script as Root](#3-run-the-script-as-root)
  - [4. Follow On-Screen Instructions](#4-follow-on-screen-instructions)
  - [5. Installation Complete](#5-installation-complete)
- [Changing Permissions (Optional)](#changing-permissions-optional)
- [Usage](#usage)
  - [1. Checking Snort Status](#1-checking-snort-status)
  - [2. Customization](#2-customization)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## Overview

This bash script automates the installation and basic configuration of Snort 3, a powerful Network Intrusion Detection System (NIDS), on your Linux system. Snort helps you monitor and detect suspicious network activities, enhancing your network's security.

## Features

- Updates your system and installs necessary packages.
- Installs LuaJIT and DAQ from source, which are required for Snort.
- Downloads and compiles the latest version of Snort from the official repository.
- Creates basic configuration files and placeholders for custom rules.
- Sets up Snort as a systemd service for continuous monitoring.
- Provides a basic test to confirm the successful installation.

## Prerequisites

Before using this script, ensure that:

- You have a Linux-based operating system.
- You are logged in as the root user or have sudo privileges.

## Installation

### 1. Clone the Repository

Start by cloning this repository to your local machine:

```bash
https://github.com/7PiNz/Snort-3-Easy-Script.git)
```

### 2. Navigate to the Script Directory

Change your current directory to the script's folder:

```bash
cd Snort-3-Easy-Script
```

### 3. Run the Script as Root

Execute the script as the root user:

```bash
sudo ./snortV.3_install.sh
```

### 4. Follow On-Screen Instructions

During the script execution, you'll be prompted to provide your `HOME_NET` configuration (e.g., '192.168.1.0/24', 'any'). Follow the on-screen instructions to input your network configuration.

### 5. Installation Complete

The script will install Snort 3, configure it, and start the Snort service. You will see a confirmation message once the installation is complete.

## Changing Permissions (Optional)

By default, the script sets the necessary permissions for execution. However, if you encounter permission issues, you can manually change permissions as follows:

1. **Navigate to the Script Directory**:

   Change your current directory to the script's folder:

   ```bash
   cd Snort-3-Easy-Script
   ```

2. **Change Permissions**:

   Use the `chmod` command to change permissions to make the script executable:

   ```bash
   chmod +x snortV.3_install.sh
   ```

   This command allows you to execute the script without the need for `sudo`.

## Usage

### 1. Checking Snort Status

To check the status of the Snort service, use the following command:

```bash
systemctl status snort.service
```

This will display the current status of Snort, including any error messages or logs.

### 2. Customization

The script provides a basic installation and configuration of Snort. You can customize the rules and configuration further according to your specific network requirements.

## Contributing

Contributions to this script are welcome! If you have improvements or bug fixes, please submit a pull request.

## Credits

- Snort 3 Easy Script Created by: 7PiNz

## License

This script is open-source and available under the [MIT License](LICENSE).
