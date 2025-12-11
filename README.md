🔍 Attack Surface Mapping Tool (Subdomain Enumeration)
Project Summary
This project simulates the external reconnaissance phase of a vulnerability assessment, a critical skill for junior security analysts and penetration testers. The goal is to map an organization's publicly exposed assets, primarily subdomains.

The application simulates the data collection and analysis steps performed after querying a public Certificate Transparency Log (CTL) like crt.sh. It demonstrates how to filter the resulting assets and flag security risks like expired certificates and exposed development infrastructure.

⚠️ Important Note on Simulation
Due to browser security restrictions (specifically CORS policies), this front-end application cannot make direct, real-time API calls to external services (like crt.sh).

The project uses hardcoded mock data to demonstrate the crucial analysis and vulnerability flagging logic that follows successful data collection. This proves competency in what to look for, even without a live proxy backend.

Valid Input Domains
To successfully run the analysis and see the generated security findings, you must use one of the following domains:

gemini.com: This domain contains a rich dataset including simulated expired certificates, wildcard domains, development/test hostnames (api-dev.), and mixed-case assets to trigger all the security findings.

example.com: This domain contains a smaller, standard set of assets, primarily used for basic functionality testing.

Any other input domain (e.g., google.com, wikipedia.org) will result in a "No assets found" message, as they are not included in the simulated dataset.

Key Skills Demonstrated for Interviewers
This project is built to demonstrate the following critical skills:

External Reconnaissance: Understanding the process of gathering public-facing asset information to map an attack surface.

Vulnerability Assessment: Ability to analyze raw data for high-priority security risks (e.g., certificate hygiene).

Certificate Analysis (SSL/TLS): Identifying and flagging issues like expired certificates, nearing expiry, and the use of wildcard certificates.

Triage and Prioritization: Categorizing findings (High Risk, Warning, Informational) to guide remediation efforts.

Running the Project
This project is a single, self-contained HTML file (subdomain_enumerator.html) and requires no backend.

Clone the repository.

Open subdomain_enumerator.html directly in any web browser.

Use one of the Valid Input Domains listed above.
