1. conf-Dateien einbinden
2. sicher stellen, dass das geo-Modul aktiviert ist
3. im Server Block:

        if ($badagent) {
                return 444;
        }

        if ($denied) {
                return 444;
        }

4. ggf. fail2ban konfigurieren
