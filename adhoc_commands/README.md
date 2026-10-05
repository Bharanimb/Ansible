Ansible Ad-Hoc Commands

This directory contains commonly used Ansible ad-hoc commands for practice and reference.

1. Connectivity
Ping all managed nodes
ansible all -i inventory -m ping -u username -k

2. File and Directory Management
Create a directory
ansible all -i inventory -m shell -a "mkdir XXX" -u username -k
Create a file
ansible all -i inventory -m shell -a "touch test.txt" -u username -k
Remove a file
ansible all -i inventory -m shell -a "rm test.txt" -u username -k
Check files in the current directory
ansible all -i inventory -m shell -a "ls -l" -u username -k

3. System Information
Check hostname
ansible all -i inventory -m shell -a "hostname" -u username -k
Check disk usage
ansible all -i inventory -m shell -a "df -h" -u username -k
Check memory usage
ansible all -i inventory -m shell -a "free -h" -u username -k
Check running processes
ansible all -i inventory -m shell -a "ps aux" -u username -k
