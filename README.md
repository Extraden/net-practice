*This project has been created as part of the 42 curriculum by dsemenov.*

# NetPractice

## Description
NetPractice is a practical introduction to computer networking.

The goal of the project is to understand and apply the fundamentals of TCP/IP networking by fixing small simulated network configurations. Through 10 levels, the learner must make each network functional by correctly setting values such as IP addresses, subnet masks, and default gateways.

This project focuses on understanding how devices communicate inside the same subnet, how routing works between different networks, and how routers and switches fit into the overall network structure.

## Instructions
### Running the training interface
1. Download the files attached to the NetPractice project page.
2. Extract them into any folder.
3. Run the provided script:

```bash
./run.sh
```

This launches a local web server and opens the NetPractice interface in your browser.

### If `run.sh` does not work
You can start the interface manually:

```bash
python3 -m http.server 49242
```

Then open your browser and go to:

```text
http://localhost:49242
```

You may use another port if needed.

### Using the interface
- Enter your 42 login to use your personal configuration.
- You can also use the **evaluation** tab to generate a random configuration.
- Each level shows a broken network and one or more goals to complete.
- Modify the available fields until the network works correctly.
- Use **Check again** to test your configuration.
- Use **Get my config** to export the current configuration.
- After a successful level, click **Next level** to continue.

### Important submission workflow
- Complete all **10 levels**.
- After each level, export the configuration with **Get my config**.
- Do **not** forget to export before moving to the next level.
- Place the **10 exported configuration files** (one per level) at the **root of the repository**.
- Only files present in the repository will be evaluated.

## What is learned in this project
NetPractice helps build a practical understanding of the following networking concepts:
- TCP/IP addressing
- IPv4 addresses
- Subnet masks
- Network and host portions of an address
- Default gateway
- Local communication inside the same subnet
- Routing between different subnets
- Routers
- Switches
- Basic packet forwarding logic
- OSI model basics, especially how addressing and routing relate to lower and network layers

## Resources
### Classic references
- RFC 791 - Internet Protocol (IPv4 fundamentals)
- RFC 950 - Internet Standard Subnetting Procedure
- Cisco Networking Academy materials on IPv4, subnetting, and routing
- MDN and similar beginner-friendly networking overviews for IP addressing and local networks
- Practical subnetting tutorials and IPv4 calculators for training and verification

### Topics worth reviewing
To be fully comfortable with the project, it is useful to revise:
- How to identify whether two hosts are in the same subnet
- How subnet masks determine the network boundary
- Why a default gateway is needed
- When a router is required
- The difference between switching and routing
- How a routing table decides where a packet goes

### How AI was used
AI was used as a support tool for:
- clarifying networking theory (subnet masks, gateways, routing logic)
- explaining mistakes found in level configurations
- reformulating documentation into a clean and readable README

AI was **not** used as a substitute for understanding. All generated explanations and text should be reviewed, verified, and fully understood before submission.

## Submission and Evaluation Notes
During peer evaluation, you will have to solve **three random levels** within a limited time.

External tools are not allowed during the evaluation. A simple calculator such as `bc` is tolerated, but that is the limit.

Because of that, it is important not only to save the exported files, but also to understand the logic behind subnetting, addressing, and routing.

## Repository Structure
Example:

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

> Replace the exported filenames above with the exact filenames produced by the NetPractice interface.
