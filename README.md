Claude Monet Bio Webpage

Quick start (Windows PowerShell)

1) Install Node.js (one-time)
- Download and install LTS from https://nodejs.org and accept defaults.

2) Install dependencies (one-time)
```powershell
cd "C:\Users\Evie\Downloads\Coding Projects\Claude Monet Bio Webpage"
npm.cmd install --no-audit --no-fund
```

3) Start local server
```powershell
# start with the project's script (uses `serve`)
npm.cmd start
# or start on a specific port:
npx serve -l 8000
```

Open in browser: http://localhost:5000 (or whichever port `serve` shows)

Alternatives
- Python 3 simple server:
```powershell
cd "C:\Users\Evie\Downloads\Coding Projects\Claude Monet Bio Webpage"
python -m http.server 8000
```
Open: http://localhost:8000

- VS Code: install "Live Server" extension and choose "Open with Live Server" on `index.html`.

Notes
- If PowerShell blocks `npm` (execution policy), using `npm.cmd` avoids the policy. To change policy (optional):
```powershell
# Run as Administrator only if you understand the implications
Set-ExecutionPolicy RemoteSigned -Scope CurrentUser
```
- To make the server accessible on other devices on your LAN, use the "On Your Network" URL `serve` prints and ensure your firewall allows incoming connections on that port.
