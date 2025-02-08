
### Test-NetConnection Cmdlet

The `Test-NetConnection` cmdlet in PowerShell is a versatile tool used to diagnose network connectivity issues. It provides detailed information about network connections, including the ability to test connectivity to a remote host, check for open ports, and perform traceroute operations. This cmdlet is essential for troubleshooting network problems and verifying network configurations.

#### Usage

To use the `Test-NetConnection` cmdlet, follow these steps:

1. Open PowerShell:
   - Press `Win + X` and select `Windows PowerShell` or `Windows PowerShell (Admin)`.

2. Type the following command and press `Enter`:
   ```
   Test-NetConnection -ComputerName <hostname_or_ip>
   ```
   Replace `<hostname_or_ip>` with the name or IP address of the remote host you want to test connectivity to. For example:
   ```
   Test-NetConnection -ComputerName google.com
   ```

The command will execute and display detailed information about the network connection to the specified host.

#### Examples

Here are some common examples of using the `Test-NetConnection` cmdlet:

- **Test Connectivity to a Remote Host**: To test basic connectivity to a remote host, type the following command and press `Enter`:
  ```
  Test-NetConnection -ComputerName google.com
  ```

- **Check for Open Ports**: To check if a specific port is open on a remote host, type the following command and press `Enter`:
  ```
  Test-NetConnection -ComputerName google.com -Port 80
  ```

- **Perform a Traceroute**: To perform a traceroute to a remote host, type the following command and press `Enter`:
  ```
  Test-NetConnection -ComputerName google.com -TraceRoute
  ```

- **Test Connectivity Using a Specific Protocol**: To test connectivity using a specific protocol, such as TCP, type the following command and press `Enter`:
  ```
  Test-NetConnection -ComputerName google.com -Port 80 -InformationLevel Detailed
  ```

#### Additional Options

The `Test-NetConnection` cmdlet supports various parameters for more advanced queries. Some common parameters include:

- `-Port`: Specifies the port number to test on the remote host.
- `-TraceRoute`: Performs a traceroute to the remote host.
- `-InformationLevel`: Specifies the level of detail to include in the output (e.g., Detailed).
- `-CommonTCPPort`: Tests connectivity to a common TCP port (e.g., HTTP, HTTPS, RDP).

These options can be useful for diagnosing specific network issues and verifying network configurations.

#### Example

To test connectivity to a remote host on port 443 (HTTPS) and display detailed information, type the following command and press `Enter`:
```
Test-NetConnection -ComputerName google.com -Port 443 -InformationLevel Detailed
```
This will display detailed information about the network connection to the specified host on port 443.

#### Additional Information

The `Test-NetConnection` cmdlet is a powerful tool for diagnosing network connectivity issues and verifying network configurations. It provides detailed insights into network connections, making it essential for IT professionals and network administrators. By using `Test-NetConnection`, users can efficiently troubleshoot network problems, check for open ports, and perform traceroute operations.
