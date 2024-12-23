# Command-Line CFG Cloner

## Overview
This program dumps the cfgspace and writemask of a PCIe device.

Note: This program is experimetal and can crash PCs under certain circumstances so be sure to save all of your work before using. Quirks are being ironed out. Some PCIe devices simply cannot be flipped, likely due to their drivers.

## Installation
1. Clone the repository:

    ```bash
    git clone https://github.com/lyk64/cli-cfg-cloner.git
    ```

2. Move cli-cfg-cloner.py to the Arbor's python folder, usually located at C:\MindShare\Arbor\python

## Usage
1. Open Arbor

2. Click Local System

3. Open the dropdown on Local System and click Rescan

4. Click PCI Config and sort by Linear

5. Note the BDF of your PCIe device. Ex: 6:0:0

6. At the top of the program, click Python Scripts

7. Click Run Script File

8. Click the Version drop down and select New Configuration

9. Set the Path to the Python 2.7 install location, usually located at C:\Python27 (Arbor uses Python 2.7 natively) (Download here: https://www.python.org/downloads/release/python-2718/)

10. Name the configuration P27

11. Browse for the script file and select the cli-cfg-cloner.py

12. Click Run

13. The cfgspace and writemask .coe files will be in the C:\MindShare\Arbor\python

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
