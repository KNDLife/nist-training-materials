# NIST SP 800‑189 Revision 1: Border Gateway Protocol (BGP) Security and Resilience

The Border Gateway Protocol (BGP) is the routing protocol that connects
networks across the internet.  It was not designed with strong security
features, which has allowed misconfigurations and malicious attacks such as
prefix hijacking and route leaks.  NIST’s **SP 800‑189r1**, released as a
public draft in early 2025, provides practical guidance for securing BGP and
improving resilience【411499849118930†L119-L145】.

## Why guidance is needed

Incidents like BGP prefix hijacking can redirect internet traffic to
attackers or disrupt services.  Large‑scale denial‑of‑service attacks often
exploit weaknesses in routing.  Federal networks, internet service
providers (ISPs) and enterprise networks all rely on BGP, so improving its
security benefits everyone【411499849118930†L119-L145】.

## Recommended practices

* **Resource Public Key Infrastructure (RPKI):** Use RPKI to issue
  cryptographic certificates that bind IP address ranges to their legitimate
  owners.  Create **Route Origin Authorizations (ROAs)** and perform
  **route origin validation** to ensure that BGP announcements come from
  authorized networks【157998376153108†L154-L172】.
* **Prefix filtering and limits:** Configure routers to filter out
  unexpected route announcements and set limits on the number of prefixes
  accepted from peers【411499849118930†L119-L145】.
* **DDoS mitigation:** Implement source address validation using access
  control lists and **unicast Reverse Path Forwarding (uRPF)** to block
  spoofed packets.  Use **remotely triggered black hole filtering** and
  **flow specification** (FlowSpec) to quickly divert or block attack
  traffic【157998376153108†L154-L172】.
* **Monitoring and coordination:** Regularly monitor BGP activity for
  anomalies and coordinate with peers and upstream providers when incidents
  occur.

## Applicability

Although the guidance is aimed at federal network operators, it is also
relevant to ISPs and enterprises.  Vendors can use it when designing
routers and security products.  Applying these measures will help secure
internet routing infrastructure against attacks and misconfigurations【411499849118930†L140-L145】.
