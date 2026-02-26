*This project has been created as part of the 42 curriculum by dsemenov.*

# NetPractice

A practical 42 project focused on learning core networking logic through small troubleshooting exercises.

## Table of Contents
- [Description](#description)
- [Instructions](#instructions)
- [Resources](#resources)
- [Evaluation Notes](#evaluation-notes)
- [Repository Layout](#repository-layout)

## Description
NetPractice is a training project designed to build a practical understanding of basic computer networking.

The project consists of **10 levels**, each showing a broken simulated network. Your job is to make the network work again by correcting the available values: mainly **IP addresses**, **subnet masks**, and **default gateways**. As the levels progress, the exercises reinforce how communication works inside a subnet, when a router is needed, and how traffic reaches another network.

This project is less about memorizing theory and more about developing the reflex to reason about:
- whether two devices are in the same subnet,
- which address is reachable directly,
- when traffic must go through a gateway,
- and how routers and switches fit into packet delivery.

## Instructions
### 1. Run the training interface
1. Download the files attached to the NetPractice project page.
2. Extract them into any folder.
3. From that folder, run:

```bash
./run.sh
```

This starts a local web server and opens the NetPractice interface in your browser.

### 2. Manual launch (if `run.sh` does not work)
If the script does not work correctly, start the interface manually:

```bash
python3 -m http.server 49242
```

Then open:

```text
http://localhost:49242
```

You may choose another port if needed.

### 3. Use the interface
- Enter your **42 login** to use your personal configuration.
- You can also use the **evaluation** tab to generate a random configuration.
- Each level displays one broken network and one or more goals.
- Modify the available fields until the network becomes valid.
- Use **Check again** to verify your solution.
- Use **Get my config** to export the current level configuration.
- Once a level is solved, continue with **Next level**.

### 4. Export configurations and submit correctly
- Complete all **10 levels**.
- Before moving to the next level, export the current one with **Get my config**.
- Export **one file per level**.
- Place all **10 exported configuration files** at the **root of the repository**.
- Keep **README.md** at the repository root as well.
- Only files present in the repository will be evaluated.

### 5. Important submission reminder
Do not forget to enter your **42 login** in the interface before exporting your files.

## Resources
### Networking concepts covered
This project explicitly studies and applies the following topics:
- TCP/IP addressing
- IPv4 addressing
- Subnet masks
- Network part vs host part of an address
- Default gateways
- Direct communication inside the same subnet
- Routing between different subnets
- Routers
- Switches
- Basic forwarding logic
- OSI layers, especially the relationship between addressing, routing, and lower-level delivery

### Classic references
- **RFC 791** - Internet Protocol
- **RFC 950** - Internet Standard Subnetting Procedure
- Cisco Networking Academy materials on IPv4, subnetting, switching, and routing
- MDN networking overviews for beginner-friendly explanations
- Practical subnetting tutorials and IPv4 calculators for training and self-checking

### How AI was used
AI was used only as a support tool for:
- clarifying networking concepts,
- checking explanations about subnetting and routing logic,
- and helping draft this README in a cleaner and more readable format.

AI was **not** used as a substitute for understanding the project. Any AI-generated explanation or text should be reviewed, verified, and fully understood before submission.

## Evaluation Notes
During peer evaluation, you will be asked to complete **three random levels** within a limited time.

External tools are not allowed during the evaluation. A simple calculator such as `bc` is tolerated, but that is the limit.

Because of that, the goal is not only to save valid exported files, but also to genuinely understand how subnetting, addressing, and gateways work.

## Repository Layout
Example structure:

```text
.
├── README.md
├── level1.json
├── level2.json
├── level3.json
├── level4.json
├── level5.json
├── level6.json
├── level7.json
├── level8.json
├── level9.json
└── level10.json
```

> Replace the example filenames above with the exact filenames exported by the NetPractice interface.
