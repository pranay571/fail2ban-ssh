# fail2ban-ssh

## Usage

### Install required packages
Debian / Ubuntu
```bash
$ sudo apt update && sudo apt install -y openssh-server fail2ban rsyslog git
```
RHEL / Fedora / CentOS
```bash
$ sudo dnf install -y openssh-server fail2ban rsyslog git
```

### Clone the repository
```bash
$ git clone https://github.com/pranay571/fail2ban-ssh.git
$ cd fail2ban-ssh
```

### Copy fail2ban configuration
```bash
$ sudo cp jail.local /etc/fail2ban
```

### Start the services
```
$ sudo systemctl start ssh
$ sudo systemctl start fail2ban
```
