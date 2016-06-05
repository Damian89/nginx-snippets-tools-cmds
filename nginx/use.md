1. conf-Dateien einbinden
2. sicher stellen, dass das geo-Modul aktiviert ist
3. in der nginx.conf:

        map_hash_bucket_size 128;
        map_hash_max_size 4096;

4. im Server Block:

        if ($badagent) {
                return 444;
        }

        if ($denied) {
                return 444;
        }

5. ggf. fail2ban konfigurieren

