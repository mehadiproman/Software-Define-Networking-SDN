# Software Defined Networking (SDN) with Mininet and OpenFlow

This repository contains a series of labs designed to introduce key Software Defined Networking (SDN) concepts using Mininet and OpenFlow. The labs guide you through building network topologies, testing connectivity, configuring programmable flows, and understanding how SDN simplifies network control.

---

## Overview

Through these labs, you will learn how to:

* Build custom network topologies in Mininet
* Simulate network behavior without physical hardware
* Test connectivity using basic tools (ping, ip, route, etc.)
* Interact with programmable flows at Layers 2, 3, and 4
* Use SDN controllers to manage the data plane

---

## Topics Covered

This repository demonstrates:

* Simulating simple network topologies
* Layer 2 OpenFlow forwarding
* Layer 3 OpenFlow forwarding
* Layer 4 OpenFlow forwarding
* Two-subnet topologies
* VLAN networks in Mininet
* ARP fundamentals and advanced ARP scenarios
* Routing across subnets
* Managing programmable network flows via SDN controllers

---

## Requirements

Before running the labs, ensure you have:

* A Linux-based system (Ubuntu recommended)
* Python 3 installed
* Basic networking knowledge (hosts, switches, ARP, routing)
* Mininet installed with a functional OpenFlow controller

---

## Installation and Setup

### 1. Install Mininet

```
sudo apt-get update
sudo apt-get install mininet
```

### 2. Verify Mininet Binary

Check that the `mn` command exists:

```
which mn
```

If empty, install Mininet with Open vSwitch support:

```
sudo apt-get install mininet openvswitch-switch openvswitch-common
```

Verify again:

```
mn --version
```

### 3. Test Default Topology

Run:

```
sudo mn
```

Expected result: Mininet CLI starts with a default controller.

If it reports missing controller support, install the test controller:

```
sudo apt-get install openvswitch-testcontroller
```

Then re-run:

```
sudo mn
```

This resolves the `Could not find a default OpenFlow controller` issue.

---
