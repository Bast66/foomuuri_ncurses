# foomuuri_ncurses
simple ncurses interface for foomuri

Features:
🎯 Vollständiger Funktionsumfang:

Zone Management (Add/Edit/Delete)
Rule Configuration mit Services
NAT Rules (DNAT/MASQUERADE)
Live Apply mit foomuuri reload

🎨 Sauberes Interface:

Farbkodierte Actions (grün=accept, rot=drop)
Pfeil-Navigation
Konfirmations-Dialogs
Error-Handling

📁 Config-Management:

Liest bestehende Foomuuri-Configs
Generiert saubere .conf-Dateien
Validierung beim Apply


Installation & Nutzung:
# Dependencies installieren
sudo apt install python3-dev  # Linux
# oder für Windows: pip install windows-curses

# Ausführen
sudo python3 foomuuri-tui.py

einfache zu erweitern:
# Neue Services hinzufügen:
COMMON_SERVICES.append("custom-service")

# Neue NAT-Typen:
nat_types = ["dnat", "snat", "masquerade", "redirect"]

# IPv6-Support:
def _add_ipv6_rule(self):
    # Easy to add!
