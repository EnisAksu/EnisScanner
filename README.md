# SCOUT v1.0
S.C.O.U.T. stands for Streamlined Cybersecurity OSINT Utiliy Tool aka SCOUT. 
SCOUT is a free tool for scanning and analyzing IPs, URLs, and file hashes using various online security services.

## Tool Objectives

SCOUT is designed to significantly reduce the time security analysts spend on OSINT (Open Source Intelligence) research during their investigations. The tool achieves this by:

- Automating Data Collection: SCOUT simultaneously queries multiple OSINT sources, eliminating the need for manual searches across different platforms.
- Centralizing Information: All relevant data is consolidated into a single CSV output, providing a comprehensive overview at a glance.
- Accelerating Decision-Making: By quickly gathering critical information, analysts can make faster, more informed decisions about potential threats.
- Enhancing Efficiency: The tool processes multiple items (IPs, URLs, hashes) in seconds, a task that would take hours if done manually.
- Standardizing Data Format: Consistent output format allows for easier integration with other analysis tools and workflows.

Key information gathered by SCOUT includes:

For Files:
- Creation time
- First submission time to VirusTotal
- Detection rates from multiple antivirus engines
- Last analysis date
- Signature verification status
- Signer company information

For Domains and URLs:
- Creation dates
- VirusTotal scan results
- URLScan.io analysis outcomes
- Google Safe Browsing status
- Recently registered domain status (within last 12 months)

For IP Addresses:
- Ownership information (Autonomous System)
- AbuseIPDB report numbers and abuse confidence percentages
- Associated domain names
- Country information

## Features

- Scans IPs using VirusTotal and AbuseIPDB
- Analyzes URLs and domains with VirusTotal and URLScan.io
- Checks file hashes against VirusTotal database
- Processes CSV files containing multiple items
- Provides an improved GUI with dark mode for easy use
- Automatically checks for and prompts for missing API keys
- Supports drag and drop functionality for CSV files

## Prerequisites

- Windows operating system
- Internet connection
- API keys for VirusTotal, AbuseIPDB, and URLScan.io

## Installation

1. Download SCOUT.exe from the releases page of this repository.

2. Obtain API keys for:
   - VirusTotal
   - AbuseIPDB
   - URLScan.io

3. The application will prompt you to enter any missing API keys on first run.

## Usage

1. Double-click SCOUT.exe to run the application.
2. Use the GUI to select your input CSV file (either by browsing or dragging and dropping).
3. Click the "SCAN" button to start the analysis.
4. Results will be saved in a new CSV file in the same directory as the input file.

## Input CSV Format

The input CSV should contain columns with IPs, URLs, or file hashes. The SCOUT will automatically detect and process these items.

## Features in v1.0

- Improved GUI with dark mode for better visibility
- Automatic API key checking and prompting
- Enhanced error handling and timeout management for API requests
- Visibility of scan progress and results
- API Keys tab to add your API Keys
- OSINT Services tab to select which OSINT resources you want to use

## Limitations and Known Issues

- The tool relies on free API tiers which may have rate limits
- The tool works best with unlimited corporate APIs
- Large CSV files may take a long time to process
- Email addresses may be mistakenly identified as domains in some cases
- Some filenames might be identified and scanned as URLs

## Important Note for First Time Use

SCOUT might be flagged by Windows Defender as this is a new program. If you see a "Windows protected your PC" message, click "More info" and then "Run anyway". This is a standard security measure for new applications downloaded from the internet. The executable is clean and safe to run.

## Disclaimer

This tool is for educational and research purposes only. Users are responsible for complying with applicable laws and the terms of service of the APIs used.

## Unlicensed

No rights reserved @EnisAksu. This tool was designed, developed and created by Enis Aksu and cannot be sold or given for monetary gain by anyone else. Otherwise, you are free to use it and improve it via its source code.
