# Privacy

AxeStation runs on your computer. No cloud account, analytics or external
telemetry service is used.

Wi-Fi passwords are used to configure selected miners and are not included in
logs. Wi-Fi setup uses the operating system's network APIs; location permission
allows Wi-Fi network names to be read, without collecting location coordinates.

Discovered devices, selections, settings, logs, Wi-Fi restoration information and
firmware caches are temporary session data, discarded on normal exit. Exported
PDFs remain wherever you save them and may include device IPs and readings.
Copy logs you need before quitting. An unexpected crash can leave temporary
files for the operating system to clean up.

Release checks contact the public GitHub update feed at startup, every six hours
and when requested. Update downloads contact GitHub release hosting. Miner
firmware checks and downloads contact the official GitHub repositories and their
release hosts. Those servers receive ordinary connection information such as
your public IP address. Shop Wi-Fi credentials are not sent to those servers.

Updating restarts AxeStation with a fresh session. Temporary installer staging
is separate from session data so installation can finish after the app closes;
successful updates clean it up after restart. Failed or interrupted updates may
leave an application backup or temporary update folder for recovery.
