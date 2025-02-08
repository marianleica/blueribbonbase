### nslookup Command Line

The `nslookup` command in Windows is a network administration tool used for querying the Domain Name System (DNS) to obtain domain name or IP address mapping information. This command is useful for diagnosing DNS-related issues and verifying DNS records.

#### Usage

To use the `nslookup` command, follow these steps:

1. Open Command Prompt:
   - Press `Win + R` to open the Run dialog.
   - Type `cmd` and press `Enter`.

2. Type the following command and press `Enter`:
   ```
   nslookup <domain>
   ```
   Replace `<domain>` with the domain name you want to query. For example:
   ```
   nslookup kurzgesagt.org
   ```

The command will execute and display the IP address associated with the specified domain name.

#### Example

To find the IP address of "kurzgesagt.org", type the following command and press `Enter`:
```
nslookup kurzgesagt.org
```
This will display the IP address associated with the domain “kurzgesagt.org”.

#### Additional Options

The `nslookup` command also supports various options and parameters for more advanced queries. Some common options include:

- `nslookup -type=mx <domain>`: Queries the mail exchange (MX) records for the specified domain.
- `nslookup -type=ns <domain>`: Queries the name server (NS) records for the specified domain.
- `nslookup -type=soa <domain>`: Queries the start of authority (SOA) records for the specified domain.

These options can be useful for obtaining specific DNS record information for troubleshooting and verification purposes.
