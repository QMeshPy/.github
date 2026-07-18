<div align="center">

<img src="https://github.com/QMeshPy.png?size=220" width="160" alt="QMeshPy" />

# QMeshPy

### Building a distributed internet for quantum computation.

We are exploring how quantum operations can become **discoverable peer-to-peer services**—routed across a global compute mesh, executed by specialized nodes, and assembled into complete scientific results.

[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB?logo=python&logoColor=white)](https://www.python.org/)
[![Qiskit](https://img.shields.io/badge/Qiskit-Quantum-6929C4?logo=ibm&logoColor=white)](https://www.ibm.com/quantum/qiskit)
[![libp2p](https://img.shields.io/badge/libp2p-Distributed-EF4B5F?logo=ipfs&logoColor=white)](https://libp2p.io/)

</div>

## The distributed quantum internet

```text
Quantum program
      ↓
Split into executable circuit fragments
      ↓
Discover compatible peers through libp2p
      ↓
Route fragments to distributed quantum services
      ↓
Execute on simulators today—and quantum processors tomorrow
      ↓
Reassemble, verify, analyze, and share results through IPFS
```

Nodes advertise capabilities through **GossipSub**, receive circuit fragments over **libp2p streams**, and return partial quantum states to a coordinator. Qiskit currently provides execution and analysis while IPFS enables content-addressed sharing of circuits and research artifacts.

## What we are working on

- **Financial modelling** — QAOA portfolio optimization, option pricing, risk analysis, and quantum-versus-classical comparisons.
- **Drug discovery** — molecular simulation, quantum chemistry workflows, candidate scoring, and distributed scientific search.
- **Scientific computing** — reusable quantum operations exposed as network services for researchers and autonomous agents.
- **Open quantum infrastructure** — peer discovery, execution planning, fault-aware routing, provenance, and independently operated compute nodes.

## Benchmark snapshot

Current Qiskit statevector experiments compare QAOA portfolio optimization with Simulated Annealing:

| Portfolio size | Classical (SA) | Quantum (QAOA) | Result |
|---:|---:|---:|---|
| 10 assets | **20 ms** | 1,500 ms | Classical 75× faster |
| 20 assets | **600 ms** | 1,700 ms | Classical 2.8× faster |
| 40 assets | 6,000 ms | **1,900 ms** | **Quantum 3.2× faster** |
| 60 assets | 20,000 ms | **2,100 ms** | **Quantum 9.5× faster** |

One important finding: roughly **97% of current QAOA runtime is classical parameter search**, not circuit execution. That means distributed nodes alone do not create quantum advantage—the opportunity comes from better optimization methods and more favorable scaling as problems grow.

> These are simulator-based research benchmarks, not claims of production quantum-hardware advantage. Results depend on the workload, solver, configuration, and machine.

<div align="center">

### Build the mesh. Route the circuit. Discover what scales.

[Explore our research](https://github.com/QMeshPy/distributed-quantum) · [View the organization](https://github.com/QMeshPy)

</div>
