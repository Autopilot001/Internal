# Internal — TryHackMe Room Notes

**Author:** Mohamed Nabil Algamoudi  
**Room:** [Internal](https://tryhackme.com/room/internal)  
**Focus:** External, web application, and internal penetration testing methodology

This repository documents my completed, authorized run of the TryHackMe **Internal** room. I used the screenshots as my working notes and placed each image beside the step it records. I have masked target and host IP addresses, credentials, and both flag values in the public copies. The screenshots are evidence of the workflow; this repository contains no secrets or executable payload files.

> **Scope:** The assigned TryHackMe room instance only.

## Walkthrough

The step-by-step narrative and screenshot gallery are in [docs/WRITEUP.md](docs/WRITEUP.md).

## Methodology

1. Enumerate exposed TCP services.
2. Discover web paths and identify the WordPress application.
3. Assess the login surface and document authorized access without publishing recovered credentials.
4. Review the application foothold and record the limited shell access shown in my notes.
5. Enumerate local files and identify the internal service lead.
6. Use SSH port forwarding to reach the internal Jenkins interface.
7. Assess the Jenkins administrative surface and document the resulting access.
8. Verify the final privilege level and record completion without disclosing flag contents.

## Lessons learned

- Treat exposed web services as an attack surface and enumerate methodically.
- Validate findings before using them to make the next decision.
- Keep testing scoped to the assigned lab.
- In a real environment, rotate exposed secrets, remove unsafe application paths, restrict administrative consoles, and segment internal services.

## Public evidence handling

Every image in `screenshots/` is a redacted PNG copy of a step screenshot I supplied. Original screenshots, credentials, IP addresses, session material, and flag values are not included.
