# modprobe command

## Overview
`modprobe` is used to load or unload Linux kernel modules.  
It automatically resolves dependencies, making it more reliable than low-level tools like `insmod`.

## Syntax
modprobe [OPTION] <module_name>

## Examples

### Load a module
$ modprobe <module_name>

### Remove a module
$ modprobe -r <module_name>

## Options
| Option | Description |
|--------|------------|
| -r | Remove (unload) a module |
| -n | Show what would be done without executing |

## Use Cases

- Manually load device drivers
- Remove problematic modules
- Reload modules during troubleshooting
- Apply configuration changes

## Practical Insight

Unlike `insmod`, `modprobe` handles module dependencies automatically.  
This makes it the preferred tool for safely managing kernel modules.

## Summary

`modprobe` is essential for controlling kernel modules and ensuring proper driver operation in Linux systems.
