# Outbox-Cron

Ruft den Nachrichtenausgang des Veluna-Portals fortlaufend auf (`Outbox-Ping`), damit
Flatfox-Anfragen sofort beantwortet und fällige Nachrichten sofort verschickt werden.

Warum dieses Repo: Vercel Hobby erlaubt nur tägliche Crons, und GitHub drosselt
Schedule-Workflows in privaten Repos stark. In einem öffentlichen Repo sind die
Actions-Minuten unbegrenzt und die Schedules deutlich zuverlässiger.

Das Zugriffs-Secret (`CRON_SECRET`) liegt in den Repository-Secrets und entspricht
der Umgebungsvariable `CRON_SECRET` im Vercel-Projekt.
