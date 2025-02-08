
### diskpart Utility

The `diskpart` utility in Windows is a command-line disk partitioning tool that allows users to manage disks, partitions, and volumes. This utility is useful for advanced disk management tasks, such as creating, deleting, and resizing partitions, as well as converting disk formats.

#### Usage

To use the `diskpart` utility, follow these steps:

1. Open Command Prompt with administrative privileges:
   - Press `Win + X` and select `Command Prompt (Admin)` or `Windows PowerShell (Admin)`.

2. Type the following command and press `Enter`:
   ```
   diskpart
   ```

The `diskpart` utility will start, and you will see the `DISKPART>` prompt, indicating that you are now in the diskpart environment.

#### Common Commands

Here are some common `diskpart` commands and their usage:

- **List Disks**: To display a list of all disks on your machine, type the following command and press `Enter`:
  ```
  list disk
  ```

- **Select Disk**: To select a specific disk, type the following command and press `Enter`:
  ```
  select disk <disk_number>
  ```
  Replace `<disk_number>` with the number of the disk you want to select.

- **List Partitions**: To display a list of all partitions on the selected disk, type the following command and press `Enter`:
  ```
  list partition
  ```

- **Create Partition**: To create a new partition, type the following command and press `Enter`:
  ```
  create partition primary size=<size_in_MB>
  ```
  Replace `<size_in_MB>` with the size of the partition in megabytes.

- **Delete Partition**: To delete a specific partition, type the following command and press `Enter`:
  ```
  delete partition
  ```

- **Format Partition**: To format a specific partition, type the following command and press `Enter`:
  ```
  format fs=<file_system> label=<label> quick
  ```
  Replace `<file_system>` with the file system type (e.g., NTFS, FAT32) and `<label>` with the volume label.

#### Example

To create a new partition on Disk 1 with a size of 10240 MB (10 GB), follow these steps:

1. Open `diskpart`:
   ```
   diskpart
   ```

2. List all disks:
   ```
   list disk
   ```

3. Select Disk 1:
   ```
   select disk 1
   ```

4. Create a new partition:
   ```
   create partition primary size=10240
   ```

5. Format the new partition as NTFS with the label "NewVolume":
   ```
   format fs=ntfs label=NewVolume quick
   ```

#### Additional Information

The `diskpart` utility is a powerful tool that should be used with caution. Incorrect usage can result in data loss or system instability. Always ensure you have backups of important data before performing disk management tasks.
