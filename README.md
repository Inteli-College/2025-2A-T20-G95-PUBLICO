How can the restructuring of specific Linux kernel components from
C to Rust effectively mitigate memory security vulnerabilities?
==

> 2025-2A-T20-G95\
> Guilherme Novaes Lima, Tomaz Mikio Sasaki

## Project Overview

The research investigates restructuring specific Linux kernel components from C to Rust to mitigate memory security vulnerabilities. The project selected the **r8169** network driver (Realtek RTL8111/8168/8411 PCI Express Gigabit Ethernet Controller) as the target component for this proof-of-concept (POC) implementation.

### Sprint 1: Project Definition

**Duration:** August 4-15, 2025

The initial sprint established the foundational framework for the research. Key deliverables included preparing the Technical Approach and Project Implementation (TAPI) form and defining the project's macro scope. The scope formalized the research question: _"How can the restructuring of specific Linux kernel components from C to Rust effectively mitigate memory security vulnerabilities?"_

The project scope was defined to focus on a single, limited Linux kernel component with criteria including functional relevance, known memory security vulnerabilities in the C implementation, and manageable complexity for migration within available resources.

### Sprint 2: Exploratory Analysis

**Duration:** August 18-29, 2025

This sprint focused on comprehensive research and component selection. The team produced three critical research reports: definition and description of the analyzed component, research on Linux driver development, and research on software engineering using Rust.

The r8169 driver was selected based on its widespread use in consumer hardware, well-documented codebase, and known memory management patterns typical of network drivers that could benefit from Rust's safety guarantees. Network drivers represent a particularly vulnerable attack surface due to their exposure to untrusted network inputs.

### Sprint 3: Deepening the Research

**Duration:** September 1-12, 2025

The third sprint delivered substantial theoretical groundwork. Major deliverables included a complete literature review on memory security in C and Rust within the kernel context, detailed analysis of the involved hardware and firmware developed in C, and definition of the restructuring methodology.

The methodology documentation detailed strategies for gradual and secure migration, including tools and techniques such as static analysis with Clippy for Rust, dynamic analysis capabilities, and interoperability approaches between C and Rust modules within the kernel environment.

### Sprint 4: Implementation Phase 1/8

**Duration:** September 15-26, 2025

Implementation began with architectural planning and environment setup. The sprint produced Rust design proposal documentation detailing the component's architecture and design, including interfaces for interoperability with C.

The development environment construction involved physical components and virtualization infrastructure, establishing the necessary toolchain including the Rust compiler (rustc), Cargo package manager, and kernel compilation tools such as GCC, Clang, and Make. This setup enabled compilation of Rust modules within the Linux kernel build system, a critical technical milestone.

### Sprint 5: Implementation Phase 2/8

**Duration:** September 29 - October 10, 2025

The fifth sprint transitioned from planning to active code development. Key deliverables included construction of basic component modules in Rust and elaboration of initial tests.

The r8169_rs repository contains the initial Rust implementation of core driver functionality. The linuxdrivers repository provides the development environment framework supporting the implementation process. Initial modules implemented fundamental driver operations while maintaining compatibility with the existing kernel infrastructure through carefully designed Foreign Function Interface (FFI) bindings.

### Sprint 6: TODO!
### Sprint 7: TODO!
### Sprint 8: TODO!
### Sprint 9: TODO!
### Sprint 10: TODO!
### Sprint 11: TODO!
### Sprint 12: TODO!
### Sprint 13: TODO!
### Sprint 14: TODO!
### Sprint 15: TODO!
### Sprint 16: TODO!
### Sprint 17: TODO!
### Sprint 18: TODO!
### Sprint 19: TODO!
### Sprint 20: TODO!
