Shopware 6 Developer Test

🚀 Schnellstart (< 1 Minute)
– VoraussetzungenDocker & Docker Compose
– Mindestens 4GB RAM
1. InstallationShopware 6 starten (bereits vorinstalliert!):
docker-compose up -d
1. 
2. Fertig! Kein Setup nötig, sofort verfügbar:
3. Shop: http://localhost
4. Admin: http://localhost/admin
5. User: admin
6. Pass: shopware
7. Mailhog: http://localhost:8025
8. Adminer: http://localhost:8888
– Was ist vorinstalliert:✅ Shopware 6 mit Demo-Daten
– ✅ Admin-User bereits angelegt
– ✅ Alle Entwickler-Tools (Composer, Node, etc.)
– ✅ Xdebug für Debugging

💻 Entwicklung
– Nach dem ersten Start:Alle Shopware-Dateien sind im shopware/ Ordner
– Plugins entwickeln: shopware/custom/plugins/
– Themes entwickeln: shopware/custom/plugins/
# Plugin-Ordner erstellen
mkdir shopware/custom/plugins/MeinPlugin

# Shopware-Befehle ausführen
docker-compose exec web bin/console plugin:refresh
docker-compose exec web bin/console plugin:install --activate MeinPlugin

# Cache leeren
docker-compose exec web bin/console cache:clear

🎯 Testaufgaben

Siehe TESTAUFGABEN.md für alle Aufgaben mit Business-Kontext.

🐛 Bei Problemen
# Container-Logs anzeigen
docker-compose logs -f web

# Alles zurücksetzen
docker-compose down -v
docker-compose up -d

Viel Erfolg! 🚀
