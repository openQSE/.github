# openQSE

**openQSE** is a community-driven initiative to define standard interfaces and architectural boundaries across the quantum–HPC software stack.

openQSE is **not** a software stack like Qiskit, PennyLane or Cirq. Instead, it focuses on identifying common software layers and defining stable, vendor-neutral interfaces between them, enabling interoperability across implementations, hardware platforms, and deployment environments.

---

## What is openQSE?

openQSE is a **standards and architecture effort**, not a monolithic software project.

- It defines **common APIs and contracts** across the quantum–HPC software stack
- It is **implementation-agnostic** and **vendor-neutral**
- It is comparable in spirit to what **MPI** did for parallel computing: enabling portability and interoperability while allowing diverse implementations and innovation

openQSE provides a shared architectural foundation on which multiple quantum software stacks and hardware platforms can interoperate.

---

## Focus: Architecture, Not Tools

openQSE concentrates on **architectural clarity and layering**, rather than prescribing specific tools or implementations.

Key activities include:

- Defining the **overall quantum–HPC software architecture**
- Identifying and describing **distinct software layers**
- Determining which layers should expose **standardized interfaces**, and which should remain implementation- or hardware-specific
- Defining **stable APIs** between layers to support portability and composability

Examples of layers under consideration include:
- Programming and front-end interfaces
- Intermediate representations (IRs)
- Compilation and transpilation
- Orchestration, runtime, and execution
- Device capability discovery
- Results, telemetry, and data interfaces

---

## Why openQSE Exists

As quantum computing moves into HPC and data center environments, facilities increasingly face the challenge of supporting:

- Multiple quantum hardware platforms
- Multiple, incompatible software stacks
- Diverse application programming models

This creates significant **integration, operational, and maintenance overhead**.

openQSE exists to address these challenges by:

- Enabling **interoperability** across software stacks and hardware platforms
- Supporting **diverse hardware deployments** without requiring a facility to rebuild its software infrastructure
- Allowing applications to use **different programming paradigms** while targeting common interfaces
- Encouraging **innovation at each layer** (front-end, compiler, runtime, hardware) without fragmenting the ecosystem
- Reducing vendor lock-in and long-term operational risk

---

## Role Relative to Existing Stacks (e.g., Qiskit)

openQSE is **complementary** to existing quantum software ecosystems.

- Qiskit, PennyLane or Cirq, and others are **full-featured implementations**
- openQSE defines the **neutral contract** that these implementations can adopt or interoperate with

openQSE does **not** replace Qiskit or any other stack. Instead, it provides:

- A common API surface that enables Qiskit to integrate more easily into **multi-vendor, multi-hardware environments**
- A way for applications built against openQSE interfaces to run across different backends with minimal changes
- Flexibility for vendors to continue innovating internally while presenting stable, interoperable interfaces externally

For hardware and software providers, this enables broader adoption in heterogeneous facilities while preserving room for differentiation.

---

## What openQSE Offers Beyond Any Single Stack

- **Vendor-neutral interfaces** that decouple applications from specific runtimes
- A consistent way to:
  - describe device capabilities
  - submit work
  - retrieve results
- The ability to **mix and match components**, such as pairing a preferred compiler or runtime with different hardware backends
- Lower integration and maintenance costs for facilities
- Improved portability and longevity for applications
- A foundation for **community governance** of shared interfaces across the quantum–HPC ecosystem

---

## Community-Driven

openQSE is developed openly and collaboratively.

Given the number of existing stacks and stakeholders, defining meaningful common interfaces requires **broad community input** from:
- HPC facilities
- Quantum hardware vendors
- Control electronics vendors
- Software framework developers
- Application scientists and users

The project evolves through discussion, working groups, and reference implementations that help validate architectural choices.

---

## Getting Involved

If you are interested in contributing to or following openQSE:
- Participate in discussions
- Join working groups as they form
- Share requirements, use cases, and lessons learned from real deployments

The goal is a practical, interoperable quantum–HPC software ecosystem that scales with both technology and community needs.
