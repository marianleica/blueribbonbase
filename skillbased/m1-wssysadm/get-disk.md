
### Get-Disk Cmdlet

The `Get-Disk` cmdlet in PowerShell is used to retrieve information about the physical disks available on a computer. This cmdlet is useful for managing and configuring disks, as well as for gathering detailed information about disk properties and status.

#### Usage

To use the `Get-Disk` cmdlet, follow these steps:

1. Open PowerShell:
   - Press `Win + X` and select `Windows PowerShell` or `Windows PowerShell (Admin)`.

2. Type the following command and press `Enter`:
   ```
   Get-Disk
   ```

The command will execute and display a list of all physical disks on your computer, along with their properties.

#### Examples

Here are some common examples of using the `Get-Disk` cmdlet:

- **List All Disks**: To display a list of all physical disks, type the following command and press `Enter`:
  ```
  Get-Disk
  ```

- **Filter by Disk Number**: To display information about a specific disk by its number, type the following command and press `Enter`:
  ```
  Get-Disk -Number <disk_number>
  ```
  Replace `<disk_number>` with the number of the disk you want to retrieve information about. For example:
  ```
  Get-Disk -Number 1
  ```

- **Filter by Operational Status**: To display disks with a specific operational status, type the following command and press `Enter`:
  ```
  Get-Disk | Where-Object OperationalStatus -eq 'Online'
  ```

#### Additional Options

The `Get-Disk` cmdlet supports various parameters for more advanced queries. Some common parameters include:

- `-CimSession`: Runs the cmdlet in a remote session or on a remote computer.
- `-FriendlyName`: Filters disks by their friendly name.
- `-PartitionStyle`: Filters disks by their partition style (e.g., MBR, GPT).

These options can be useful for narrowing down the list of disks and finding exactly what you need.

#### Example

To display detailed information about all online disks, type the following command and press `Enter`:
```
Get-Disk | Where-Object OperationalStatus -eq 'Online'
```
This will display a list of all online disks along with their detailed properties.

#### Additional Information

The `Get-Disk` cmdlet is an essential tool for PowerShell users, providing a comprehensive way to explore and manage physical disks on a computer. It helps users understand the capabilities of their storage devices and perform various disk management tasks efficiently.
