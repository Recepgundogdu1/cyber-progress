# Cybersecurity Progress Log (private)

Kişisel ilerleme kaydım. Çözdüğüm oda/makineleri, harcadığım saati ve
kısa notları buraya işliyorum. Detaylı çözümler public `security-writeups`
reposunda.

## Özet
- Başlangıç: 2026-10-19
- Toplam oda/makine: 12
- Toplam saat: ~15
- Güncel streak: 7 gün

## Günlük Log

| Tarih      | Platform | Oda/Makine                     | Zorluk    | Saat | Portföy? | Kısa Not |
|------------|----------|--------------------------------|-----------|------|----------|----------|
| 2026-10-20 | THM      | Search Skills                  | Easy      | 0.5  | Hayır    | Isınma, biliyordum |
| 2026-10-21 | THM      | Guided Pentest: Web            | Easy      | 2    | Evet     | IDOR → upload bypass → RCE zinciri |
| 2026-10-21 | THM      | Guided Pentest: Infrastructure | Easy      | 2    | Evet     | UnrealIRCd exploit → root privesc |
| 2026-10-22 | THM      | Dive Into Pentesting           | Info/Easy | 1.5  | Hayır    | Teori: metodoloji, risk (V×T=R), ethics/permission/trust |
| 2026-10-22 | THM      | Cyber Kill Chain               | Medium    | 1    | Hayır    | Teori: Lockheed Martin 7 aşama (Recon → ... → Actions on Objectives) |
| 2026-10-23 | THM      | Penetration Testing Frameworks | Easy      | 1.5  | Hayır    | Teori: OSSTMM, WSTG, NIST 800-115, PTES, ISSAF, ATT&CK + framework seçimi |
| 2026-10-23 | THM      | Passive Reconnaissance         | Easy      | 1    | Hayır    | Pratik: whois/RDAP, nslookup/dig (TXT flag), DNSDumpster, crt.sh, Shodan |
| 2026-10-24 | THM      | Active Reconnaissance          | Easy      | 0.75 | Hayır    | Netcat/telnet ile banner grabbing; HTTP server+sürüm, FTP (21) sürüm tespiti, curl -I Server header |
| 2026-10-24 | THM      | Protocols and Servers          | Easy      | 1    | Hayır    | HTTP/FTP/SMTP/POP3/IMAP elle (telnet/nc); banner grabbing, cleartext insecurity teması |
| 2026-10-24 | THM      | Protocols and Servers 2        | Easy      | 1    | Hayır    | Auth saldırıları (Hydra), sniffing/MITM, SSH hardening, Wireshark protokol filtreleri (imap vb.) |
| 2026-10-25 | THM      | Nmap Live Host Discovery       | Easy      | 1    | Hayır    | Host discovery: -sn, ARP (-PR), ICMP (-PE/-PP/-PM), TCP SYN/ACK ping, -n/-R/--dns-servers |
| 2026-10-26 | THM      | All in One                     | Easy*     | 1.5  | **Evet** | Çok vektörlü CTF. Zincir: mail-masta LFI (php://filter → wp-config DB creds) → WP admin → functions.php reverse shell → www-data → gizli dosyadan (find -user) elyana şifresi → sudo socat (GTFOBins) → root. Bir sürü çıkmaz sokak + pivot. |

\* "Easy" etiketli ama pratikte baya zorladı — çoklu yol, çok sayıda kapalı vektör.

## Kolonlar ne demek
- **Portföy?**: Evet = public repoda writeup yazılacak/yazıldı
- **Kısa Not**: tek satır özet — detay writeup'ta
