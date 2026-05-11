# nslookup google.com

## Screenshot
![nslookup-google](../../../screenshots/Linux/networking/nslookup-google.png)

## Command Used

```bash
nslookup google.com
```

## What It Does
Queries DNS servers to resolve domain names into IP addresses.

## Why It Is Used
Support technicians use nslookup to troubleshoot:
- DNS issues
- website resolution problems
- connectivity issues
- incorrect DNS settings

## Real Job Example
A user reports websites are not loading properly.
A technician uses `nslookup` to verify whether DNS is resolving domain names correctly.

## Difference Between Windows and Linux
The command works similarly on both Windows and Linux systems, although the output formatting may differ slightly.

Windows and Linux both use DNS servers to translate domain names into IP addresses.

## My Result
My Kali Linux VM successfully resolved `google.com` into the IP address:

```text 
142.251.32.174
```

This confirmed that DNS resolution was functioning properly on my Kali Linux VM.

## What I Learned
I learned how DNS converts domain names into IP addresses and how technicians verify DNS functionality using the `nslookup` command.

## Notebook Short Notes
- nslookup tests DNS
- Converts website names into IP addresses
- Used when websites fail to load
- DNS = phonebook of the internet
