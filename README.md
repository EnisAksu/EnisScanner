# Enis Scanner
Enis Scanner is a free tool for scanning and analyzing IPs, URLs, and file hashes using various online security services.

## Features
- Scans IPs using VirusTotal and AbuseIPDB
- Analyzes URLs and domains with VirusTotal and URLScan.io
- Checks file hashes against VirusTotal database
- Processes CSV files containing multiple items
- Provides a simple GUI for easy use

## Prerequisites
- Windows operating system
- Internet connection
- API keys for VirusTotal, AbuseIPDB, and URLScan.io

## Installation
1. Download EnisScanner.exe from the releases page of this repository.

2. Obtain API keys for:
   - VirusTotal
   - AbuseIPDB
   - URLScan.io

3. Set up environment variables for your API keys:
   - Open Command Prompt as Administrator
   - Run the following commands, replacing with your actual API keys:
     ```
     setx VTCLI_APIKEY "your_virustotal_api_key"
     setx ABUSEIPDB_APIKEY "your_abuseipdb_api_key"
     setx URLSCAN_APIKEY "your_urlscan_api_key"
     ```
   - Restart your computer for the changes to take effect

## Usage
1. Double-click EnisScanner.exe to run the application.

2. Use the GUI to select your input CSV file and start the scan.

3. Results will be saved in a new CSV file in the same directory as the input file.

## Input CSV Format
The input CSV should contain columns with IPs, URLs, or file hashes. The scanner will automatically detect and process these items.

## Limitations and Known Issues
- The tool relies on free API tiers which may have rate limits
- The tool best works with unlimited corporate APIs
- Large CSV files may take a long time to process
- Email addresses may be mistakenly identified as domains in some cases
- Some filenames might be identified and scanned as URLs

## Disclaimer
This tool is for educational and research purposes only. Users are responsible for complying with applicable laws and the terms of service of the APIs used.

## License
All rights reserved @EnisAksu. This tool was designed, developed and created by Enis Aksu and cannot be sold or given for free by anyone else.
