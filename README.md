# Internal — TryHackMe Room Notes

**Author:** Mohamed Nabil Algamoudi  
**Room:** [Internal](https://tryhackme.com/room/internal)  
**Focus:** External, web application, and internal penetration testing methodology

This repository documents my completed, authorized run of the TryHackMe **Internal** room. I used the screenshots as my working notes and placed each image beside the step it records. I have masked target and host IP addresses, credentials, and both flag values in the public copies. The screenshots are evidence of the workflow; this repository contains no secrets or executable payload files.

> **Scope:** The assigned TryHackMe room instance only.

## work

The narrative and screenshot gallery are in [docs/WRITEUP.md](docs/WRITEUP.md).

## Methodology

I began by mapping exposed services and discovering the WordPress site, then assessed its login surface and documented the application foothold. From there, I reviewed local files for the internal Jenkins lead, used SSH port forwarding to reach that service, and documented the later access and privilege verification while keeping credentials and flags private.

## Lessons learned

- Treat exposed web services as an attack surface and enumerate methodically.
- Validate findings before using them to make the next decision.
- Keep testing scoped to the assigned lab.
- In a real environment, rotate exposed secrets, remove unsafe application paths, restrict administrative consoles, and segment internal services.
