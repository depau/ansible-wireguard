# Ansible WireGuard role

This role makes it easy to set up WireGuard on a number of machines.

## Features

- Supports both `wg-quick` and `systemd-networkd` configs
- Supports IPv4 and IPv6
- Supports having one node as a gateway to the Internet
- Supports having one node that forwards packets to the Internet only for one
  protocol suite (i.e. to add IPv6 connectivity to machines that don't have it)
- Supports having one node as an internal router, to have devices without a
  static public endpoint communicate without any issues.
- Additional hosts (not configured with Ansible) can be added to the network
- <s>Supports basic firewall configuration with UFW</s> - Removed since I don't use UFW any more and the code was nasty anyway


## Usage

Well commented examples are available in [.examples](.examples).

You need to add this as a role and include it in a playbook.


## License

This repo is licensed under the GNU GPLv3.0 license.

This work is the result of many months of bashing my head into it to solve
weird edge cases, and I still think it's not perfect. If you find it useful,
please contribute back your suggestions ♥
