# Disable Windows Update Permanently Using CMD

This guide provides instructions to permanently stop and disable Windows Update on a Windows machine using Command Prompt (CMD).

## Steps to Disable Windows Update

### 1. Open Command Prompt as Administrator

- Press `Win + X` and select `Command Prompt (Admin)` or `Windows PowerShell (Admin)`.
- Alternatively, you can press `Win + R`, type `cmd`, and press `Ctrl + Shift + Enter`.

### 2. Stop the Windows Update Service

To stop the Windows Update service immediately, type the following command and press `Enter`:

```shell
net stop wuauserv
```
### 3. Disable the Windows Update Service

To prevent the service from starting automatically, use this command:

```shell
sc config wuauserv start= disabled
```
# Re-enabling Windows Update Permanently Using CMD

### 1. Open Command Prompt as Administra

Follow the same steps as above to open Command Prompt with administrative privileges.

### 2. Enable the Windows Update Service

To configure the Windows Update service to start automatically, use this command:

```shell
sc config wuauserv start= auto
```
### 3. Start the Windows Update Service

To start the Windows Update service immediately, type the following command:

```shell
net start wuauserv
```
