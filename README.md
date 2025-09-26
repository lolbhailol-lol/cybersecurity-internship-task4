# Task 4 - Setup and Use a Firewall (Linux UFW)

## Objective
Configure and test basic firewall rules to allow or block traffic using UFW on Linux.

## Steps Performed
1. Installed and enabled UFW firewall.
2. Checked and listed current firewall rules.
3. Added rule to block inbound traffic on port 23 (Telnet).
4. Verified the block rule.
5. Added rule to allow SSH traffic on port 22.
6. Verified rules again.
7. Deleted the block rule to restore original state.
8. Performed final verification.

## Commands Used
```bash
sudo apt install ufw -y
sudo ufw status
sudo ufw enable
sudo ufw status numbered
sudo ufw deny 23
sudo ufw status numbered
sudo ufw allow 22
sudo ufw status numbered
sudo ufw delete <rule_number>
sudo ufw status verbose
