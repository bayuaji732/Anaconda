# Anaconda Installation Guide for Multi User

## Operating System
CentOS 7

## Anaconda Installation Path
`/opt/anaconda3`

## Step-by-Step Installation Guide

1. **Create Anaconda Group:**
    ```bash
    sudo groupadd anaconda
    ```

2. **Set Group Ownership to Anaconda:**
    ```bash
    sudo chgrp -R anaconda /opt/anaconda3
    ```

3. **Set Permissions for Anaconda Directory:**
    ```bash
    sudo chmod 770 -R /opt/anaconda3
    ```

4. **Add User to Anaconda Group:**
    ```bash
    sudo usermod -a -G anaconda <username>
    ```

## Note:
- Ensure that the Anaconda installation directory is `/opt/anaconda3`.
- Replace `<username>` with the actual username you want to add to the Anaconda group.

---
