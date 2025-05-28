# IT Technikus Vizsgasegédlet

Ez a nyilvános jegyzettár segít a technikumi ágazati vizsgára való felkészülésben. A cél, hogy gyorsan visszakereshető, érthető, jól rendszerezett példák álljanak rendelkezésre.

**A tartalmak általános tudásanyagot tartalmaznak, nem konkrét vizsgamegoldásokat!**

## Informatika és Távközlés

**Linux parancsok:**
```
ip a                   # hálózati beállítások
sudo apt update       # csomaglista frissítése
sudo systemctl restart apache2  # szolgáltatás újraindítása
chmod +x script.sh    # futtathatóvá tétel
```

**SQL parancsok:**
```sql
SHOW TABLES;  -- táblák listázása
SELECT nev FROM dolgozok WHERE fizetes > 300000;
INSERT INTO dolgozok (nev, fizetes) VALUES ('János', 280000);
```

---

## Cisco Packet Tracer

**Router IP-cím beállítása:**
```
enable
configure terminal
interface FastEthernet0/0
ip address 192.168.1.1 255.255.255.0
no shutdown
```

**Alapvető konfiguráció:**
```
hostname Router1
copy running-config startup-config
ip route 0.0.0.0 0.0.0.0 192.168.1.254
```

**Switch VLAN konfigurálás:**
```
interface FastEthernet0/1
switchport mode access
switchport access vlan 10
vlan 10
name HR
```

---

## Python

**Fájlkezelés:**
```python
with open("adatok.txt", "r", encoding="utf-8") as f:
    for sor in f:
        print(sor.strip())
```

**Szótár rendezése érték szerint:**
```python
ertekek = {"Anna": 5, "Béla": 9, "Cecil": 7}
for nev in sorted(ertekek, key=ertekek.get, reverse=True):
    print(nev, ertekek[nev])
```

**Fájl létezésének ellenőrzése:**
```python
import os
if os.path.exists("adatok.txt"):
    print("Megvan a fájl!")
```

---

## HTML és CSS

**Alap HTML oldal:**
```html
<!DOCTYPE html>
<html>
<head>
    <title>Példa oldal</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <h1>Üdvözlet!</h1>
    <p>Ez egy példa HTML oldal.</p>
</body>
</html>
```

**Egyszerű CSS stílus:**
```css
body {
    font-family: Arial, sans-serif;
    background-color: #f2f2f2;
    color: #333;
}
h1 {
    color: darkblue;
}
```

---

## Hasznos linkek és eszközök

- [GitHub](https://github.com/)
- [Regex tesztelő](https://regex101.com/)
- [Shell parancs elemző](https://explainshell.com/)
- [IP kalkulátor](https://www.subnet-calculator.com/)
- [Markdown szerkesztő](https://dillinger.io/)

---

**Használat:**
- Gyakorláshoz, ismétléshez, tanórákon és vizsga előtt

**Tanároknak:** Szabadon megosztható, kinyomtatható, QR-kód formájában is elérhető

**PDF és QR-kód verzió kérhető!**
