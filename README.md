# ProtonVPN Secure Core CLI Shortcut

This small Bash CLI tool connects to a predefined list of ProtonVPN Secure Core servers.

It is designed for Linux users who use the ProtonVPN CLI and want a quick, simple command to connect to privacy-friendly Secure Core routes without manually selecting servers every time.

Secure Core routes traffic through a hardened Proton-owned server (for example in Switzerland or Iceland) before exiting in another country. This adds an extra protection layer if an exit server is monitored or seized.

More about Secure Core:
https://protonvpn.com/vpn-servers#secure-core

## Selected privacy-friendly countries

The following countries were selected based on general privacy reputation and legal environment.  
This is a personal selection, not an official ranking.

- Switzerland
- Iceland
- Norway
- Sweden
- Romania
- Finland
- Estonia
- Luxembourg

## Secure Core routes used

- Austria: CH-AT#2 (to connect to my own country)
- Estonia: SE-EE#1, CH-EE#2
- Luxembourg: CH-LU#2
- Norway: IS-NO#1, SE-NO#1, CH-NO#2
- Finland: SE-FI#1, CH-FI#2
- Romania: SE-RO#1, CH-RO#1, CH-RO#2

## Features

- Random Secure Core connection
- Interactive menu
- Quick disconnect
- Minimal setup

## Usage

Make the file executable:

```bash
chmod +x vpn
```

Run the commands:

Connect to a random VPN server in the list:
```bash
~$ vpn
```

Disconnect from the current vpn connection:
```bash
~$ vpn -d
```

List all selected Secure Core Servers:
```bash
~$ vpn -l
```

Get a selection menu to connect to a specific server:
```bash
~$ vpn -d
```

Show all these commands in your terminal:
```bash
~$ vpn -h
```

> **Important:** This also needs the ProtonVPN CLI installed. My tool is just a shortcut but not the main product:
https://protonvpn.com/support/linux-vpn-setup