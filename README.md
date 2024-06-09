# Configuration for macOS on Workstation
###### If you ever want to install macOS on VMware Workstation, you'll have to use this. For the full installation guide, head [here](https://www.link.com). For [The VMware Center](https://www.youtube.com/@VMwareCenter).
1. Go to the Workstation folder for your macOS VM
2. Find the .VMX file and open it with Notepad (or any other text editing software)
3. At the bottom of the file, paste in these lines of code according to your CPU.

### For Intel CPUs
```smc.version = "0"```

```smbios.reflectHost = "TRUE"```

```hw.model = "MacBookPro14,3"```

## For AMD CPUs
```smc.version = "0"```

```cpuid.0.eax = "0000:0000:0000:0000:0000:0000:0000:1011"```

```cpuid.0.ebx = "0111:0101:0110:1110:0110:0101:0100:0111"```

```cpuid.0.ecx = "0110:1100:0110:0101:0111:0100:0110:1110"```

```cpuid.0.edx = "0100:1001:0110:0101:0110:1110:0110:1001"```

```cpuid.1.eax = "0000:0000:0000:0001:0000:0110:0111:0001"```

```cpuid.1.ebx = "0000:0010:0000:0001:0000:1000:0000:0000"```

```cpuid.1.ecx = "1000:0010:1001:1000:0010:0010:0000:0011"```

```cpuid.1.edx = "0000:0111:1000:1011:1111:1011:1111:1111"```

```smbios.reflectHost = "TRUE"```

```hw.model = "MacBookPro14,3"```
