# Distributed System

### Definition
A distributed system is a collection of seperate and independernt software/hardware components, called nodes, that are networked and work together coherently by coordincating and communicating through messages passing or events, to fulfill one end goal.

Nodes can be unstructure or highly structured, depending on the system requirements. The complexities are hidden away from the end user, making the whole system appear as one computer.

Examples: Pass, Iaas, etc.

### Main Characteristics

1. No shared clock between nodes.
2. No shared memory between nodes.
3. Tasks are executed concurrerently.
4. Heterogeneity and Loose Coupling.
5. Dynamic with Overlay Networks.

### Other Concepts

1. Nodes have their own processors and could be hardware/software, forming open or
closed groups.
2. Resource is an asset that's accessed remotely. It could be virutally anything, such as files, services, storage, other networks, etc.
3. Distribution Transparency is to keep as much of the system as hidden as possible, from the user. This is done through a middleware.
4. Middleware is a logical layer on top of the collective nodes. It handles communication, security, failures, etc. It can be though of as the backbone of the system.
5. Concurrency is the parallel completion of multiple tasks and operations. It is an intrinsic property of distributed systems.
6. Coordination is the smooth collaboration between operations and events.
Synchronzaion orders and controls resource sharing.
