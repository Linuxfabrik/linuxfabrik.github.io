---
hide:
  - navigation
  - toc
---

# Linuxfabrik Open Source

[Linuxfabrik](https://www.linuxfabrik.ch/) is a Swiss Linux and open source engineering company. Everything on this page is developed for our own production environments first, then released for everyone else running the same stack.

Documentation for each project lives under `linuxfabrik.github.io/<project>/`. Source, issues and releases are on [GitHub](https://github.com/Linuxfabrik).


## Projects

<div class="grid cards" markdown>

-   :material-clipboard-check-outline:{ .lg .middle } **ChecklistFabrik**

    ---

    Generates interactive HTML checklists from YAML templates. Jinja conditionals, reusable includes, pluggable modules and a built-in web server. For SOPs, deployments and recurring operations.

    [:octicons-arrow-right-24: Documentation](https://linuxfabrik.github.io/checklistfabrik/) &middot;
    [:simple-github: Repository](https://github.com/Linuxfabrik/checklistfabrik)

-   :material-wall-fire:{ .lg .middle } **FirewallFabrik**

    ---

    Successor to fwbuilder: a Qt GUI for managing iptables and nftables policies. Central policy database with reusable objects, scales to hundreds of firewalls, generates deployment-ready shell scripts.

    [:octicons-arrow-right-24: Documentation](https://linuxfabrik.github.io/firewallfabrik/) &middot;
    [:simple-github: Repository](https://github.com/Linuxfabrik/firewallfabrik)

-   :material-ansible:{ .lg .middle } **LFOps**

    ---

    Ansible Collection of roles, playbooks and plugins for Linux-based cloud infrastructure. Covers OS hardening, MariaDB, Icinga 2, Nextcloud, FreeIPA, KVM and more, with Bitwarden and cloud integration.

    [:octicons-arrow-right-24: Documentation](https://linuxfabrik.github.io/lfops/) &middot;
    [:simple-github: Repository](https://github.com/Linuxfabrik/lfops)

-   :material-language-python:{ .lg .middle } **lib**

    ---

    Python modules shared by all Linuxfabrik projects: database access, SQLite key-value caching, WinRM, SMB, shell execution and more than 15 API integrations. Available on PyPI.

    [:octicons-arrow-right-24: Documentation](https://linuxfabrik.github.io/lib/) &middot;
    [:simple-github: Repository](https://github.com/Linuxfabrik/lib)

-   :material-server-network:{ .lg .middle } **MCP Server for Icinga**

    ---

    Model Context Protocol server that lets AI clients triage and operate Icinga through the Icinga 2 Core, Icinga Web and Icinga Director REST APIs, aware of the monitoring plugins catalog.

    [:octicons-arrow-right-24: Documentation](https://linuxfabrik.github.io/mcp-server-icinga/) &middot;
    [:simple-github: Repository](https://github.com/Linuxfabrik/mcp-server-icinga)

-   :material-monitor-dashboard:{ .lg .middle } **Monitoring Plugins**

    ---

    Several hundred check, notification and event plugins for Icinga, Nagios and friends. Python 3.9+, all platforms, smart defaults, auto-discovery and consistent cross-platform metrics.

    [:octicons-arrow-right-24: Documentation](https://linuxfabrik.github.io/monitoring-plugins/) &middot;
    [:simple-github: Repository](https://github.com/Linuxfabrik/monitoring-plugins)

</div>


## More on GitHub

These repositories have no documentation site of their own. Their READMEs cover the ground.

<div class="grid cards" markdown>

-   **[github-project-createrepo](https://github.com/Linuxfabrik/github-project-createrepo)**

    Downloads RPM release assets from GitHub and builds an RPM repository with `createrepo`.

-   **[icingaweb2-theme-linuxfabrik](https://github.com/Linuxfabrik/icingaweb2-theme-linuxfabrik)**

    Icinga Web 2 theme in Linuxfabrik colors.

-   **[kickstart](https://github.com/Linuxfabrik/kickstart)**

    Unattended installations for RHEL/Fedora (Kickstart), Debian (Preseed) and Ubuntu (Autoinstall). BIOS and UEFI, automatic disk detection, four install types, locked root, LVM, SELinux enforcing.

-   **[mirror](https://github.com/Linuxfabrik/mirror)**

    Creates and updates mirrors of RPM repositories using `reposync`.

-   **[openvpn-2fa-easyrsa](https://github.com/Linuxfabrik/openvpn-2fa-easyrsa)**

    Manages OpenVPN users, their Easy-RSA certificates and TOTP-based 2FA codes, including QR code generation.

-   **[packaging](https://github.com/Linuxfabrik/packaging)**

    Build pipeline that turns Linuxfabrik's own and third-party software into RPM and DEB packages for repo.linuxfabrik.ch.

-   **[stig](https://github.com/Linuxfabrik/stig)**

    Security Technical Implementation Guides, implemented in Python for auditing and Ansible for remediation.

</div>


## Elsewhere

- [www.linuxfabrik.ch](https://www.linuxfabrik.ch/) -- company website, products and enterprise support.
- [docs.linuxfabrik.ch](https://docs.linuxfabrik.ch/) -- our German-language knowledge base for Linux system engineers.
- [repo.linuxfabrik.ch](https://repo.linuxfabrik.ch/) -- RPM and DEB package repositories.
- [download.linuxfabrik.ch](https://download.linuxfabrik.ch/) -- release artifacts and assets.


## Support and Contributing

Bug reports and feature requests belong in the issue tracker of the respective repository. Contribution rules are the same everywhere and are documented in [Contributing](contributing.md).

If a project saves you time, consider [sponsoring](https://github.com/sponsors/Linuxfabrik) its maintenance. Commercial [support and SLAs](https://www.linuxfabrik.ch/en/products/service-support) are available.
