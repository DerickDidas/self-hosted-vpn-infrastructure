# Deployment Journey

A chronological account of the project, written from memory. No logs or configs survive, so there are no exact dates or measurements beyond the subscription period.

1. **Provisioning.** Set up a RackNerd KVM VPS with Ubuntu and connected over SSH using PuTTY.
2. **WireGuard.** Deployed WireGuard as the first implementation, configured client access, and tested on smartphones, Windows computers and other devices.
3. **Connectivity problem.** The original VPS IP became unreliable for the intended connections. I researched possible network restrictions, including discussions on Chinese-language forums, but could not confirm the cause.
4. **Replacement IP.** Obtained a replacement IP for the VPS and continued experimenting.
5. **Alternative protocols.** Researched VMess and VLESS as alternative approaches.
6. **Further deployments.** Deployed and tested OpenVPN, Hiddify Manager and 3X-UI, using Docker for several of them.
7. **Testing.** Compared connection establishment, reliability, speed and latency across devices, informally.
8. **Outcome.** In my testing, Hiddify Manager gave the most successful connectivity results.
9. **End of project.** The subscription expired on March 16, 2025.
