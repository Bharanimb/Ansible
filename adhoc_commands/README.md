# Ansible Ad-Hoc Commands

This directory contains commonly used Ansible ad-hoc commands for practice and reference.

---

## 1. Connectivity

### Ping All Managed Nodes

```bash
ansible all -i inventory -m ping -u username -k
```

---

## 2. File and Directory Management

### Create a Directory

```bash
ansible all -i inventory -m shell -a "mkdir XXX" -u username -k
```

### Create a File

```bash
ansible all -i inventory -m shell -a "touch test.txt" -u username -k
```

### Remove a File

```bash
ansible all -i inventory -m shell -a "rm test.txt" -u username -k
```

### Check Files in the Current Directory

```bash
ansible all -i inventory -m shell -a "ls -l" -u username -k
```

---

## 3. System Information

### Check Hostname

```bash
ansible all -i inventory -m shell -a "hostname" -u username -k
```

### Check Disk Usage

```bash
ansible all -i inventory -m shell -a "df -h" -u username -k
```

### Check Memory Usage

```bash
ansible all -i inventory -m shell -a "free -h" -u username -k
```

### Check Running Processes

```bash
ansible all -i inventory -m shell -a "ps aux" -u username -k
```

