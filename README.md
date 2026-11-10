TriWave: Last-Mile IoMT Fetal Monitor
Overview:
The TriWave is a low-cost, portable Internet of Medical Things (IoMT) cardiotocography (CTG) monitor that bridges the diagnostic gap between rural midwives and remote specialists. By combining robust hardware sensors with an offline-capable, localized digital platform, it enables the real-time detection and management of fetal distress in resource-constrained, off-grid environments.

Technical Stack:

Hardware Sensors: C++ for embedded systems and real-time biometric data capture.

Frontend Dashboard: React.js for a responsive, multi-language telemedicine interface (Hausa, Igbo, Yoruba, Pidgin, English).

Backend & API: Node.js for managing data routing, secure storage, and clinical alerts.

Connectivity: Local URL edge-computing for offline data synchronization, utilizing local Area Networks (LAN) and buffered cloud transmission.

System Architecture:
The TriWave data pipeline is engineered specifically to bypass rural infrastructure barriers, ensuring continuous care even without active internet:

Mother (Edge Capture): Continuous biometric data (fetal heart rate and maternal contractions) is captured via sensors during labor.

TriWave Device: The hardware processes the raw sensor data in real-time.

Local LAN (Offline Sync): Data is transmitted to a local edge server/router. Frontline midwives instantly view this data on a mobile device via a local URL without requiring broadband internet.

Cloud Server: As soon as cellular connectivity is detected, the buffered edge data securely syncs to the centralized cloud gateway.

Obstetrician (Remote Triage): Specialized OB/GYNs access the web dashboard at urban command centers to review the CTG data, immediately transmitting life-saving clinical feedback and referral alerts back to the rural midwife.

Pilot Status:
The TriWave has advanced past prototyping into active field testing across five primary healthcare locations in Jigawa State, Nigeria. We have actively monitored 187 pregnant women, achieving a 62% success rate in proactively identifying fetal distress and resolving severe childbirth complications through rapid specialist intervention.

IP Notice:Note: The core source code and hardware schematics are omitted from this public repository to protect active patents and proprietary intellectual property. Full technical audits can be provided to grant reviewers upon request under an NDA.
