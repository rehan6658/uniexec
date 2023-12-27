# UniExec - Command Execution Tool

[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

## Overview

UniExec is a Python script designed for executing commands on remote machines using various connection methods. It supports methods such as 'winrm', 'ssh', 'smb', 'ldap', 'ftp', 'wmi', 'rdp', 'vnc', and 'mssql'. Additionally, it includes a local execution method ('execute_command').

## Features

- Execute commands on remote machines or locally.
- Support for multiple connection methods.
- Secure handling of credentials (optional).
- Basic exception handling for error reporting.

## Usage

### Prerequisites

- Python 3.x installed on your machine.

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/<your-username>/uniexec.git

    Change into the project directory:

    bash

    cd uniexec

Running the Tool

Run the script from the command line:

bash

python uniexec.py <command> <remote_address> [--method <method>] [--username <username>] [--password <password>] [--domain <domain>]

    <command>: The command to execute.
    <remote_address>: The address of the remote machine.
    --method <method>: The method to use for the connection (default: 'execute_command'). Other methods include 'winrm', 'ssh', 'smb', 'ldap', 'ftp', 'wmi', 'rdp', 'vnc', 'mssql'.
    --username <username>: The username for remote machine connection (optional).
    --password <password>: The password for remote machine connection (optional).
    --domain <domain>: The domain for remote machine connection (optional).

Example

bash

python uniexec.py "dir" 192.168.1.100 --method ssh --username user --password pass

This example demonstrates running the tool to execute the "dir" command on a remote machine with the address "192.168.1.100" using the SSH connection method.
Contributing

If you'd like to contribute to this project, please follow the Contributing Guidelines.
License

This project is licensed under the MIT License - see the LICENSE file for details.
