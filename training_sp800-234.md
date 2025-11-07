# NIST SP 800‑234: High‑Performance Computing Security Overlay

High‑performance computing (HPC) systems power scientific research and
large‑scale data analysis.  These systems have unique architectures and
performance requirements that make applying general security controls
challenging.  NIST’s **SP 800‑234** provides a security overlay tailored for
HPC environments【970646824201038†L430-L475】.

## Key concepts

* **Four zones:** The overlay divides an HPC system into **Access**,
  **Management**, **Computing** and **Data Storage** zones.  Each zone has its
  own services and threats, so security controls are tailored accordingly【970646824201038†L430-L475】.
* **Control baseline:** The overlay starts with the **moderate baseline** from
  SP 800‑53B and then modifies or adds controls to fit HPC needs.  It uses
  five levels of tailoring: controls that apply to all zones, plus
  additional controls specific to each zone【970646824201038†L430-L475】.
* **Added controls and notation:** Table 1 of the document summarizes 287
  controls, indicating where guidance has been added (marked “G”), where
  detailed discussions are included (“D”) and where new controls are added
  (“N”)【970646824201038†L513-L535】.  New controls like **AC‑10 (Concurrent
  Session Control)** are included for certain zones.

## Why a special overlay

HPC systems often prioritize performance over security.  Traditional
firewalls or monitoring tools may introduce unacceptable delays.  By
categorizing the system into zones and tailoring controls, SP 800‑234
helps organizations strike a balance between protecting resources and
maintaining high throughput.  Researchers and IT staff can use the overlay
as a checklist to ensure that their HPC environment is secure without
hindering the science it supports【970646824201038†L430-L475】.
