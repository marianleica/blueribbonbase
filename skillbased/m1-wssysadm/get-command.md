
### Get-Command Cmdlet

The `Get-Command` cmdlet in PowerShell is a versatile tool used to discover and display information about cmdlets, functions, workflows, aliases, and executables available in your PowerShell environment. This cmdlet is useful for exploring the capabilities of PowerShell and finding the commands you need to accomplish specific tasks.

#### Usage

To use the `Get-Command` cmdlet, follow these steps:

1. Open PowerShell:
   - Press `Win + X` and select `Windows PowerShell` or `Windows PowerShell (Admin)`.

2. Type the following command and press `Enter`:
   ```
   Get-Command
   ```

The command will execute and display a list of all available commands in your PowerShell session.

#### Examples

Here are some common examples of using the `Get-Command` cmdlet:

- **List All Commands**: To display a list of all available commands, type the following command and press `Enter`:
  ```
  Get-Command
  ```

- **Filter by Command Type**: To display only cmdlets, type the following command and press `Enter`:
  ```
  Get-Command -CommandType Cmdlet
  ```

- **Search by Name**: To find a specific command by name, type the following command and press `Enter`:
  ```
  Get-Command -Name <command_name>
  ```
  Replace `<command_name>` with the name of the command you want to find. For example:
  ```
  Get-Command -Name Get-Process
  ```

- **List Commands from a Specific Module**: To display commands from a specific module, type the following command and press `Enter`:
  ```
  Get-Command -Module <module_name>
  ```
  Replace `<module_name>` with the name of the module. For example:
  ```
  Get-Command -Module Microsoft.PowerShell.Management
  ```

#### Additional Options

The `Get-Command` cmdlet supports various parameters for more advanced queries. Some common parameters include:

- `-Verb`: Filters commands by verb (e.g., Get, Set, New).
- `-Noun`: Filters commands by noun (e.g., Process, Service, Item).
- `-Syntax`: Displays the syntax of the specified command.

These options can be useful for narrowing down the list of commands and finding exactly what you need.

#### Example

To find all commands related to services, you can use the `-Noun` parameter:
```
Get-Command -Noun Service
```
This will display a list of all commands that have "Service" as their noun, such as `Get-Service`, `Start-Service`, and `Stop-Service`.

#### Additional Information

The `Get-Command` cmdlet is an essential tool for PowerShell users, providing a comprehensive way to explore and discover the commands available in your environment. It helps users understand the capabilities of PowerShell and find the right commands for their tasks.
