# Cyber-Security-
Penetration Testing Scripts

## Ethical Penetration Testing Helper

`ethical_pentest.py` is a modular Python script for **authorized security assessments only**.

### Available modules
- `resolve`: DNS/hostname resolution
- `scan`: basic TCP port scanning
- `banner`: banner grabbing from TCP services
- `headers`: HTTP response header inspection
- `tls`: TLS certificate metadata inspection

### Usage
```bash
python ethical_pentest.py --authorized resolve example.com
python ethical_pentest.py --authorized scan scanme.nmap.org --ports 22,80,443
python ethical_pentest.py --authorized banner scanme.nmap.org 22
python ethical_pentest.py --authorized headers https://example.com
python ethical_pentest.py --authorized tls example.com
```

The script will refuse to run unless `--authorized` is provided.
