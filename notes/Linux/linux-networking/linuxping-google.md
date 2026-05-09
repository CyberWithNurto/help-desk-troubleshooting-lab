# ping google.com on Kali Linux

## Screenshot
![linuxping-google](../../../screenshots/Linux/networking/linuxping-google.png)

## Command Used

```bash
ping google.com
```

## What It Does
Tests communication between the Linux system and an external server.

## Why It Is Used
Support technicians use ping to test:
- internet connectivity
- DNS functionality
- packet communication
- network response

## Real Job Example
A user reports websites are not loading.
A technician uses ping to verify whether the system can reach external servers.

## Difference Between Windows and Linux
Windows ping sends a limited number of requests automatically.

Linux ping continues running until manually stopped using:
```bash
CTRL + C
```

## My Result
My Kali Linux VM successfully communicated with google.com and received network responses.

## What I Learned
I learned how Linux systems test connectivity to external servers and verify internet access.

## Notebook Short Notes
- ping tests connectivity
- If ping works = network likely working
- Linux ping runs continuously
- Stop using CTRL + C
