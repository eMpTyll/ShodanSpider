
# ShodanSpider v2

**ShodanSpider v2** is an advanced, powerful, and easy-to-use tool for interacting with Shodan's vast database of internet-connected devices. Ideal for cybersecurity researchers, penetration testers, and bug hunters, this tool allows users to search and analyze devices on the internet with enhanced capabilities. The tool can be used both with and without a Shodan API key for basic or premium results, making it versatile for all users.

## Features

- **Free and Open Source**: No API key required for basic use, with limited results. You can still perform Shodan searches for free but can upgrade to the full version using your Shodan API key for enhanced results.
- **Enhanced Search with API Key**: Input your Shodan API key for premium access and more detailed results, including advanced filtering and additional information.
- **Customizable Output**: Save search results to an output file and use them for later analysis. You can specify the file name to store results in a variety of formats.
- **Efficient and Fast**: Search Shodan for specific devices, vulnerabilities (CVE), and more, all while optimizing the search speed with timeouts and custom parameters.
- **Multiple Search Options**: Search for general queries, CVEs, and specific device types, making it perfect for bug hunting and vulnerability research.

## Installation

### Prerequisites

To run ShodanSpider, ensure that the following are installed:

- **bash** (for running the script)
- **curl** (for making HTTP requests)
- **jq** (for query encoding)
- **Optional**: A Shodan API key for enhanced results

### Steps to Install

1. Clone the repository:
   ```bash
   git clone https://github.com/shubhamrooter/ShodanSpider.git
   ```

2. Navigate to the project directory:
   ```bash
   cd ShodanSpider
   ```

3. Give execute permission to the script:
   ```bash
   chmod +x shodanspider
   ```

4. Optionally, make the script executable globally (optional):
   ```bash
   sudo cp shodanspider.sh /usr/local/bin/shodanspider
   ```

## Usage

Once installed, you can use **ShodanSpider v2** directly from the terminal with various options for flexible search and output control.

### Options

- `-q <query>`: Perform a Shodan search with a specific query (e.g., `apache`, `ssl`, `cve-2021-34473`, etc.).
- `-cve <cve-id>`: Search for a specific CVE (e.g., `cve-2021-34473`).
- `-o <output_file>`: Save the search results to a specified output file. If not provided, the results will be displayed on the terminal.
- `-h`: Display the help menu and available options.

### Example Commands

- **Search for 'apache' on Shodan without an API key**:
  ```bash
  ./shodanspider.sh -q "apache"
  ```

- **Search for a CVE (e.g., `cve-2021-34473`)**:
  ```bash
  ./shodanspider.sh -cve "cve-2021-34473"
  ```

- **Search for 'apache' and save results to a file**:
  ```bash
  ./shodanspider -q "apache" -o "results.txt"
  ```


- **Search for a specific CVE and save to a file**:
  ```bash
  ./shodanspider -cve "cve-2021-34473" -o "cve_results.txt"
  ```
  ![image](https://github.com/user-attachments/assets/3792c18e-1650-4ee6-9a0f-37cd2a190ec2)


## Contributing

Contributions are welcome! If you want to contribute to ShodanSpider's development, feel free to fork the repository, make your changes, and submit a pull request.

### How to Contribute

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes.
4. Commit your changes (`git commit -am 'Add new feature'`).
5. Push to your fork (`git push origin feature-branch`).
6. Submit a pull request.

## License

This tool is open-source and available under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Contact

For any questions or support, you can contact me at:

- **Email**: info@shubhamrooter.com
- **GitHub**: [ShubhamTiwari](https://github.com/shubhamrooter)

## Disclaimer

**ShodanSpider v2** is intended for educational, research, and ethical use only. Unauthorized scanning and accessing systems without proper consent may violate legal regulations. Use this tool responsibly and at your own risk.
