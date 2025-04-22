# SendEmail

## Requirements (for TLS)

### Debian/Ubuntu

```bash
sudo apt update
sudo apt install libnet-ssleay-perl libio-socket-ssl-perl
```

### CentOS/RHEL/Fedora

```bash
sudo dnf install perl-Net-SSLeay perl-IO-Socket-SSL
```

If it is an old version of CentOS:

```bash
sudo yum install perl-Net-SSLeay perl-IO-Socket-SSL
```

# Sending e-mail

```bash
./sendEmail.pl \
  -f noreply@example.com \
  -u user \
  -m message \
  -t destination@example.com \
  -s your-mail-server.example.com \
  -o tls=yes \
  -xu smtp-user \
  -xp smtp-pass
```
