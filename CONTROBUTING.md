# Contributing to xDuinoRails (Thor)

Thank you for your interest in contributing! We are building a high-performance, industry-ready decoder. Your expertise in electronics and firmware helps us push the boundaries of open-source engineering.

To maintain a high standard of quality and ensure that the project can be used in certified commercial environments (our **Seal of Approval** program), we follow a structured contribution process.

---

## 1. Legal Framework (CLA)
To protect both the project and its users, we require all contributors to sign our **Contributor License Agreement (CLA)**. 

> ### Why do we require a CLA?
> * **Dual-Licensing:** It allows us to keep the core project open-source while offering commercial licenses for partners who cannot use the reciprocal (CERN-OHL-S) license.
> * **Certification:** It ensures a clean IP provenance, which is mandatory for partners seeking our **"Seal of Approval"**.

### How to sign?
We use a **CLA Assistant bot**. When you open your first Pull Request, the bot will provide a link to a one-click digital signature via your GitHub account.

---

## 2. Technical Standards
As an engineering project involving PCB design and Firmware, we maintain strict quality controls:

### 🛠 Electronics & PCB (KiCad)
* **Version:** Use **KiCad 8.0** (or the current stable release).
* **Libraries:** Use project-specific symbols and footprints in `/libs`.
* **Verification:** All submissions must pass **ERC** (Electrical Rules Check) and **DRC** (Design Rules Check) without errors.
* **Mechanical:** Provide a **3D model (STEP format)** for any new footprints.

### 💻 Firmware (C/C++)
* **Style:** Follow the [LLVM Coding Standards](https://llvm.org/docs/CodingStandards.html).
* **Safety:** Code should be MISRA-C compliant where applicable.
* **Efficiency:** Focus on non-blocking, interrupt-driven logic suitable for real-time decoding.

### 📄 Documentation
* Update the `/docs` folder for every change (e.g., updated **BOM**, wiring diagrams, or API changes).

---

## 3. The Contribution Workflow

1. **Fork** the repository and create your branch from `main`.
2. **Commit** your changes using [Conventional Commits](https://www.conventionalcommits.org/) (e.g., `feat(hw): add input protection circuit`).
3. **Test** your changes! For KiCad, ensure the netlist is consistent and the layout is manufacturable.
4. **Open a Pull Request** against the `main` branch.
5. **Sign the CLA** via the bot comment in your PR.
6. **Review:** Maintainers will review your design for technical merit and compliance.

---

## 4. Community & Support
Questions? Open an **Issue** or join our [Discord/Slack/Forum Link]. 

*Happy Engineering!*
