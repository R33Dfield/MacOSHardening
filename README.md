# MacOSHardening

Welcome to MacOSHardening – your go-to repository for enhancing the security of macOS 14.0 Sonoma clients managed through Microsoft Intune.

## About This Repository
<img align="right" src="https://rietveld-ict.nl/wp-content/uploads/2023/12/shield_small.png"/>

This repository contains JSON and custom .mobileconfig files designed to improve macOS 14.0 Sonoma security via Microsoft Intune. The configuration settings are based on the baselines provided by CIS, following the industry-recognized [CIS Benchmarks](https://www.cisecurity.org/benchmark/apple_os) for macOS hardening. There are CIS Level 1 and Level 2 configuration files available.

It's important to note that the settings catalog in Intune does not cover all the security controls required by the CIS benchmark for macOS 14 Sonoma. To address this gap, you'll need to import the .mobileconfig files using the "Profile Templates > Custom" option in Intune. These additional files supplement the settings catalog, ensuring a more comprehensive alignment with the CIS benchmarks.

You have the flexibility to choose the approach that best suits your needs. If you use the JSON file, everything will be imported automatically but you will miss some hardening. Alternatively, you can opt to import the configurations based on the .mobileconfig files. This allows you to fine-tune them as needed to meet your organization's specific security and operational requirements.

## What's Inside
* JSON Hardening File: There is only one file based on Settings Catalog, offering you a plug-and-play solution for immediately enhancing your system's security posture. The Settings Catalog provides some settings that are listed in the CIS Benchmark. Most configuration has to be done with the .mobileconfig files (Custom Template in Intune).
* Custom .mobileconfig Files: Created using the toolset available at [NIST's macOS Security GitHub repository](https://github.com/usnistgov/macos_security), these files provide additional configuration options and security measures.
* Wide Compatibility: Primarily designed for macOS 14.0 Sonoma, these hardening files should be compatible and effective on older versions of macOS.
* A .pdf file that provides detailed documentation of all the settings included in .mobileconfig files. This file is designed to serve as a comprehensive reference guide, explaining each setting in detail. 

### How to Use
* Download: Select and download the JSON file and .mobileconfig files based on your needs.
* Import to Intune: Easily import these files into your Microsoft Intune environment.
* Create a new config policy using profile type "Templates" > template name "Custom" > import the .mobileconfig file.
* Apply Settings: Deploy these settings across your macOS Sonoma clients to enforce a robust security framework.

### Why CIS Benchmarks?
CIS Benchmarks are globally recognized as a gold standard for securing IT systems and data against cyber threats. By aligning the hardening files with these benchmarks, as much as possible, this provides you with a trustworthy and effective way to harden your macOS environments against vulnerabilities. The free available PDF files and NIST repo have been a source for building the Intune configuration files.

### Create your own baseline for macOS?
Check out the excelent video from [NIST](https://youtu.be/pYDfrYQrfqc)

## Contribution
Feel free to contribute, suggest improvements, or report issues. Your input is valuable in making "MacOSHardening" a robust and community-driven tool for Apple macOS security.

## Stay Secure
Remember, security is an ongoing journey, not a destination. Keep your systems updated and regularly check back for the latest hardening files.

## Disclaimer
Before using the configurations in the "macOSHardening" repository for Apple macOS 14 Sonoma, please test them thoroughly in your environment. Adjustments may be needed to meet your organization's specific security and operational needs. Deployment in a production environment is at your own responsibility.

## Reference
https://www.cisecurity.org/benchmark/apple_os

https://downloads.cisecurity.org/#/

