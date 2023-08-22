# Linux Privilege Escalation

Linux Privilege Escalation is not as complex as Windows. I'd recommend running the known automation scripts before you start exploiting.&#x20;

## Automation Tools

### **LinEnum**

```
-k Enter keyword
-e Enter export location
-t Include thorough (lengthy) tests
-r Enter report name
-h Displays this help text
```

{% @github-files/github-code-block url="https://github.com/rebootuser/LinEnum" %}

### Dirty Sock

{% @github-files/github-code-block url="https://github.com/initstring/dirty_sock/blob/master/dirty_sockv1.py" %}

## **Abusing Permission Issue**

**Find suid and guid files**

```
#Find SUID
find / -perm -u=s -type f 2>/dev/null

#Find GUID
find / -perm -g=s -type f 2>/dev/null
```

{% embed url="https://gtfobins.github.io/" %}

## Searching files

```
search -f *.txt
search -f *.zip
search -f *.doc
search -f *.xls
search -f config*
search -f *.rar
search -f *.docx
search -f *.sql

.ssh:
.bash_history

/var/mail
/var/spool/mail
```
