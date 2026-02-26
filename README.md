*This project has been created as part of the 42 curriculum by dsemenov.*

# NetPractice

## Description

NetPractice is a practical introduction to computer networking built around 10 small training levels.

The goal of the project is to understand how a network works by fixing broken simulated configurations. Each level requires the learner to make communication possible by setting the correct values for IP addresses, subnet masks, and default gateways.

Through these exercises, the project develops a practical understanding of local communication inside the same subnet, communication between different subnets, and the role of routing in making a network function properly.

## Instructions

### Running the training interface

1. Download the files attached to the NetPractice project page.
2. Extract them into any folder of your choice.
3. From that folder, run:

```bash
./run.sh
```

This script launches a local web server and opens the training interface in your web browser.

### Manual launch

If `run.sh` does not work properly, you can start the interface manually by running:

```bash
python3 -m http.server 49242
```

Then open the following address in your browser:

```text
http://localhost:49242
```

You may use another port if needed.

### Using the interface

- Enter your 42 login to use your personal configuration.
- You can also use the **evaluation** tab to generate a random configuration.
- Each level shows a non-working network and one or more goals to complete.
- Modify the available fields until the network works correctly.
- Use **Check again** to verify your configuration.
- Use **Get my config** to export the current level configuration.
- Before moving to the next level, export the file for the level you have just completed.

### Exporting configurations

A configuration file must be exported for each level using the **Get my config** button.

Do not skip this step before going to the next level, because the exported files are required for submission.

## Submission details

For submission, you must place **10 exported configuration files** - **one per level** - at the **root of the repository**.

- Do not place them inside a subdirectory.
- Use the exact files exported by the NetPractice interface.
- Only files present in the repository will be evaluated during the defense.
- Make sure you enter your login in the training interface before exporting the files.

## Resources

### Classic references

- RFC 791 - Internet Protocol (IPv4)
- RFC 950 - Internet Standard Subnetting Procedure
- Cisco Networking Academy materials on IPv4 addressing, subnetting, switching, and routing
- Introductory networking documentation and tutorials covering TCP/IP fundamentals
- IPv4 subnetting practice material and subnet calculators for self-checking

### Networking concepts studied

This project is based on the following networking concepts:

- TCP/IP addressing
- IPv4 addresses
- Subnet masks
- Network and host portions of an address
- Default gateways
- Routers
- Switches
- Communication inside the same subnet
- Communication between different subnets
- Basic routing logic
- OSI layers, especially the concepts related to switching and routing

### How AI was used

AI was used as a support tool for:

- clarifying networking theory such as subnet masks, default gateways, and routing decisions
- helping explain mistakes found while solving the training levels
- improving the wording and structure of this README

AI was not used as a substitute for understanding. All explanations and exported configurations were reviewed and verified manually.

## Peer-evaluation note

During the defense, you will have to complete **three random levels** within a limited time.

External tools are not allowed during evaluation. A simple calculator such as `bc` is tolerated, but no more than that.
