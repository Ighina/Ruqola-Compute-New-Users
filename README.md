# Ruqola Project Compute Resources

Welcome to the central information page for the compute resources available to the NUS, NTU, and Oxford University joint **Ruqola project**. This guide provides an overview of the available servers and instructions on how to access them.

The resources are distributed across the partner institutions, offering different scales of computational power to suit your experimental needs.

---

## The Hopper (NUS)

**The Hopper** is the primary high-performance computing (HPC) cluster for the project, provided by NUS. This server is designed and reserved for **computationally intensive experiments**, large-scale model training, and heavy data processing.

### Access Instructions

Access is a multi-step process involving (1) getting an NUS guest account, (2) activating it, (3) applying for HPC access, and (4) connecting. Please follow these instructions carefully.

#### Part 1: Requesting an NUS Guest Account

1.  Get in touch with **Prof Lee Wee Sun (School of Computing, NUS)**. He will contact NUS administrative staff to request a guest account and internal NUS email address for you.
2.  The administrative staff will contact you asking for the following information:
    * Last Name or Surname
    * First Name
    * Display Name
    * Title
    * Visitor Job Title
    * Visitor Organization
    * Organization Address
    * Email
    * Mobile Country Code
    * Mobile Number
    * Purpose of Access
    * Required Period
3.  You will receive a confirmation email with your account start date.
4.  On the **Account Start Date**, you will receive:
    * An email with a PIN-protected PDF (ePasswordSlip) containing your password.
    * An SMS with the PIN to open the PDF.

#### Part 2: Activating Your NUS Account

Before you can use the account (or apply for HPC access), you **must** complete the following steps *in sequence*:

1.  **Change Password:** Change the temporary password at [https://exchange.nus.edu.sg/passwordportal](https://exchange.nus.edu.sg/passwordportal).
2.  **Accept Policy:** Log in at [https://inetapps.nus.edu.sg/aup](https://inetapps.nus.edu.sg/aup) (using your new password) and accept the **NUS IT Acceptable Use Policy (AUP)**. This must be done within **14 days** of your account start date, or the account will be locked.
3.  **Set up MFA:** Complete the Microsoft Multifactor Authentication (MFA) setup. Follow *Section 2: Register for Multifactor Authentication (MFA)* of the [NUS-ID - Getting Started guide](https://nusit.nus.edu.sg/services/account-and-access/account/nus-id-getting-started/).

#### Part 3: Applying for Hopper (HPC) Access

1.  Once your NUS account is fully active (Parts 1 & 2 are complete), you can apply for cluster access.
2.  Fill in the form at: [https://nusit.nus.edu.sg/hpc/get-an-hpc-account/](https://nusit.nus.edu.sg/hpc/get-an-hpc-account/)
3.  In the form, use the following project name: **`CFP01-SF-001`**

#### Part 4: Connecting and User Guide

For full instructions on connecting and using the cluster, please refer to the **`Hopper Cluster User Guide.pdf`** file located in this repository.

**Quick Tips:**
* **VPN Required:** You must use the **NUS VPN (Cisco)**. Download instructions are available here (requires NUS login): [NUS VPN Guide](https://nusit-dwp.onbmc.com/dwp/app/#/knowledge/KBA00027608/rkm)
* **Project Contacts:** Wei and Duy are on the project and can advise on connecting.
* **Check Access:** After connecting via VPN, log in and run `hpc project` to verify you are in the project group.
* **Job Scheduler:** The cluster uses **PBS Pro**, not Slurm.
* **Storage:** Use **/scratch** for large local storage and virtual environments. Avoid `/hpctmp`.
* **Multi-Node Jobs:** These require MPI and a separate worker script (unlike Slurm). See the User Guide for details.

### Hopper Specifications

* **No. of GPU Nodes:** 46 nodes
* **GPU Type (per node):** 8x NVIDIA H100 80GB or 8x NVIDIA H200 141GB
* **CPU Type (per node):** 2 x Intel 8480+ 56-cores
* **Memory (per node):** 2 TB
* **Network:**
    * Infiniband NDR (400Gb) – GPU to GPU
    * Ethernet 100GbE – Storage Fabric
* **Storage:**
    * **(Scratch) BeeGFS:** 200TB
    * **(Home & Project) Dell-EMC Isilon:** 1.6PB

---

## Mjölnir (NTU)

**Mjölnir** is a smaller server provided by NTU. This resource is intended for **light-weight experiments**, such as developing proofs of concept, initial exploratory data analysis, and running smaller-scale experimental tests.

* **Access Instructions:** Coming Soon
* **Usage**: For using the server refer to the following guide [https://ighina.github.io/ruqola-server-deploy/](https://ighina.github.io/ruqola-server-deploy/)

### Mjölnir Specifications

* **GPUs:** 3x NVIDIA H200 (80GB HBM3e each)
* **Total GPU Memory:** 240GB
* **CPU:** 1 single CPU
* **Storage:** 3.4TB (Total)
* **Queue Management:** Features a custom fair resource allocation system.
