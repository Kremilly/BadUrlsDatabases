# BadUrlsDatabases

## Overview

This repository contains a collection of SQL files that list hundreds of thousands of malicious and pornographic websites. The purpose of this database is to provide security researchers, developers, and network administrators with a resource to help identify and block these types of sites, enhancing online safety and security.

## Contents

The repository includes the following files:

- `malwares.sql`: Contains URLs and metadata for websites known to host malicious content, such as malware, phishing schemes, and other security threats.
- `porns.sql`: Contains URLs and metadata for websites hosting pornographic content, intended for use in content filtering applications.
- `ips.sql`: A comprehensive list of malicious IP's.

## Structure

Each SQL file is structured as follows:

- **URL**: The web address of the site.
- **Category**: Classification of the site (e.g., "malicious", "pornographic").
- **Description**: A brief description of why the site is included in the list.
- **Date Added**: The date the URL was added to the database.
- **Additional Metadata**: Any other relevant information, such as IP addresses, domain registration details, etc.

## Usage

To use the database, follow these steps:

1. **Clone the repository**:
   ```sh
   git clone https://github.com/kremilly/BadUrlsDatabases.git
   cd BadUrlsDatabases
   ```

2. **Import the SQL files into your database**:
   You can use a tool like `mysql` or `psql` (depending on your database system) to import the SQL files. For example, with MySQL:
   ```sh
   mysql -u username -p database_name < malwares.sql
   mysql -u username -p database_name < porns.sql
   mysql -u username -p database_name < ips.sql
   ```

## Applications

This database can be used in various applications, including but not limited to:

- **Web Filtering**: Implement content filters to block access to malicious and pornographic websites.
- **Security Research**: Analyze and study patterns in malicious sites to improve security measures.
- **Parental Controls**: Develop tools to restrict access to inappropriate content for children.
- **Network Monitoring**: Monitor network traffic to identify and block requests to known harmful sites.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
