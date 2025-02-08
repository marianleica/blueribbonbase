
### Hyper-V PowerShell Module

The Hyper-V PowerShell module provides a set of cmdlets for managing Hyper-V virtual machines, virtual hard disks, and other virtualization components. This module is essential for automating and scripting Hyper-V management tasks.

#### Usage

To use the Hyper-V PowerShell module, follow these steps:

1. Open PowerShell with administrative privileges:
   - Press `Win + X` and select `Windows PowerShell (Admin)`.

2. Import the Hyper-V module if it is not already imported:
   ```
   Import-Module Hyper-V
   ```

3. Use the available cmdlets to manage Hyper-V components.

#### Examples

Here are some common examples of using the Hyper-V PowerShell module:

- **List All Virtual Machines**: To display a list of all virtual machines on the host, type the following command and press `Enter`:
  ```
  Get-VM
  ```

- **Start a Virtual Machine**: To start a specific virtual machine, type the following command and press `Enter`:
  ```
  Start-VM -Name <vm_name>
  ```
  Replace `<vm_name>` with the name of the virtual machine you want to start. For example:
  ```
  Start-VM -Name "MyVM"
  ```

- **Stop a Virtual Machine**: To stop a specific virtual machine, type the following command and press `Enter`:
  ```
  Stop-VM -Name <vm_name>
  ```

- **Create a New Virtual Machine**: To create a new virtual machine, type the following command and press `Enter`:
  ```
  New-VM -Name <vm_name> -MemoryStartupBytes <memory_size> -NewVHDPath <vhd_path> -NewVHDSizeBytes <vhd_size>
  ```
  Replace `<vm_name>`, `<memory_size>`, `<vhd_path>`, and `<vhd_size>` with the appropriate values. For example:
  ```
  New-VM -Name "NewVM" -MemoryStartupBytes 2GB -NewVHDPath "C:\VMs\NewVM.vhdx" -NewVHDSizeBytes 20GB
  ```

#### Additional Options

The Hyper-V PowerShell module supports various cmdlets for more advanced management tasks. Some common cmdlets include:

- `Get-VM`: Retrieves information about virtual machines.
- `Set-VM`: Configures virtual machine settings.
- `Remove-VM`: Deletes a virtual machine.
- `Get-VHD`: Retrieves information about virtual hard disks.
- `Optimize-VHD`: Optimizes a virtual hard disk.

These cmdlets can be useful for automating and scripting complex Hyper-V management tasks.

#### Example

To retrieve detailed information about a specific virtual machine, type the following command and press `Enter`:
```
Get-VM -Name "MyVM" | Format-List *
```
This will display detailed information about the virtual machine named "MyVM".

#### Additional Information

The Hyper-V PowerShell module is an essential tool for administrators managing Hyper-V environments. It provides a comprehensive set of cmdlets for automating and scripting virtualization tasks, making it easier to manage virtual machines and other Hyper-V components efficiently.
