# Ruqola-Compute-New-Users
A guide for new users of the various compute available for the Ruqola project
# Ruqola Project Compute Resources

Welcome to the central information page for the compute resources available to the NUS, NTU, and Oxford University joint **Ruqola project**. This guide provides an overview of the available servers and instructions on how to access them.

The resources are distributed across the partner institutions, offering different scales of computational power to suit your experimental needs.

---

## The Hopper (NUS)

**The Hopper** is the primary high-performance computing (HPC) cluster for the project, provided by NUS. This server is designed and reserved for **computationally intensive experiments**, large-scale model training, and heavy data processing.

* **Access Instructions:** For onboarding and access, please follow the instructions at: [https://nusit.nus.edu.sg/hpc/hopperonboarding/](https://nusit.nus.edu.sg/hpc/hopperonboarding/)

### Hopper Specifications

The Hopper is a powerful cluster with the following specifications:

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

* **Access Instructions:** For setup and deployment instructions, please refer to the guide at: [https://ighina.github.io/ruqola-server-deploy/](https://ighina.github.io/ruqola-server-deploy/)

### Mjölnir Specifications

* **GPUs:** 3x NVIDIA H200 (80GB HBM3e each)
* **Total GPU Memory:** 240GB
* **CPU:** 1 single CPU
* **Storage:** 3.4TB (Total)
* **Queue Management:** Features a custom fair resource allocation system.
