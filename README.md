# Enis Scanner
Enis Scanner is a free tool for scanning and analyzing IPs, URLs, and file hashes using various online security services. 

## Tool Objectives

EnisScanner is designed to significantly reduce the time security analysts spend on OSINT (Open Source Intelligence) research during their investigations. The tool achieves this by:

1. Automating Data Collection: EnisScanner simultaneously queries multiple OSINT sources, eliminating the need for manual searches across different platforms.

2. Centralizing Information: All relevant data is consolidated into a single CSV output, providing a comprehensive overview at a glance.

3. Accelerating Decision-Making: By quickly gathering critical information, analysts can make faster, more informed decisions about potential threats.

4. Enhancing Efficiency: The tool processes multiple items (IPs, URLs, hashes) in seconds, a task that would take hours if done manually.

5. Standardizing Data Format: Consistent output format allows for easier integration with other analysis tools and workflows.

Key information gathered by EnisScanner includes:

- For Files:
  * Creation time
  * First submission time to VirusTotal
  * Detection rates from multiple antivirus engines

- For Domains:
  * Creation dates
  * Associated IP addresses

- For IP Addresses:
  * Ownership information
  * AbuseIPDB report numbers and abuse confidence percentages

- For URLs:
  * VirusTotal scan results
  * URLScan.io analysis outcomes
  * Google Safe Browsing status

By automating the collection of this crucial OSINT data, EnisScanner empowers analysts to focus on higher-level threat analysis and decision-making, rather than time-consuming data gathering. This tool can potentially reduce OSINT research time from hours to mere minutes, significantly improving the efficiency and effectiveness of security investigations.

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

## Important Note for first time use
EnisScanner might be stopped by Defender as this is my very first program, I did not have much experience to make more Defender friendly one.
If you see "don't run" button on the bottom right, then click "More Info" link and then "Run anyway". As you have downloaded this executable from internet, this is a defense mechanism by Defender. However, as the executable is clean, it allows you to run it.

## Disclaimer
This tool is for educational and research purposes only. Users are responsible for complying with applicable laws and the terms of service of the APIs used.

## License
All rights reserved @EnisAksu. This tool was designed, developed and created by Enis Aksu and cannot be sold or given for free by anyone else.
