# Proxmox Cloud-init Template Downloader

This bash script facilitates the downloading and setup of Cloud-init OS templates for Proxmox Virtual Environment (PVE). It automates the download of specified operating system images and imports them into Proxmox as VM templates, streamlining the process of creating new VMs with various operating systems.

## Features

The script supports a predefined list of cloud-init enabled OS images, which currently includes:
- Debian 10 (EOL - No Support)
- Debian 11
- Debian 12
- Ubuntu Server 20.04
- Ubuntu Server 22.04
- Alma Linux 8
- Alma Linux 9

## Prerequisites

- A Proxmox VE installation.
- Internet connectivity to download OS images.
- Sufficient storage space in your desired storage location for the image files.

## Usage

1. Downloading the script:

    ```bash
    wget https://raw.githubusercontent.com/HOKOHOST/Proxmox-Cloudinit-Template-Downloader/main/osdl.sh
    ```

2. Ensure the `osdl.sh` script is executable:

    ```bash
    chmod +x osdl.sh
    ```

3. Run the script as the root user (or with sudo privileges) on your Proxmox server:

    ```bash
    ./osdl.sh
    ```

4. Follow the on-screen prompts to:
    - Select the desired operating system.
    - Specify the target storage location.
    - Assign a VMID for the new template.
  
5. The script will handle the rest!

## Interactive Prompts

You will be prompted for the following information:
1. **Operating System Selection**: Choose from the predefined list of supported OS templates.
2. **Target Storage**: Enter the target storage ID (e.g., 'local').
3. **VMID**: Assign a VMID that is not already in use on your Proxmox server.

## Contributions

Your contributions are most welcome. Feel free to make improvements by submitting pull requests.

## Support

This script is provided by [HOKOHOST](https://hokohost.com/scripts). If you find it valuable and wish to support further development or say thanks, please consider making a donation at [HOKOHOST Donate](https://hokohost.com/donate). Your support is greatly appreciated.

## License

This project is licensed under the [MIT License](LICENSE) - see the LICENSE file for details.

## Disclaimer

This script is provided 'as-is', without any warranty or guarantee of any kind. Use it at your own risk.

## Author Information

This script is proudly presented to you by [HOKOHOST](https://hokohost.com). Stay updated with the latest versions by visiting our website.
