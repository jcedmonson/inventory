## Installation / Download / Initial Deployment

1. Install Windows Subsystem for Linux

   - Open Powershell
   - `wsl --install`

2. Download Docker Desktop @ https://www.docker.com/
3. Install Docker Desktop (recommended settings)
4. Download Git Repo as Zip
5. Extract into Downloads
6. Open PowerShell
7. Navigate to downloads directory
8. Run
   `docker compose up`

## Deploy

`docker compose up`

## Configure PGAdmin

1. Navigate to PGAdmin exposed @ port 3000
2. Login with demo@demo.com, demo
3. Add new Server (quick links)
   - General - Name: Inventory
   * Connection - Hostname: system IP
   * Connection - Username: postgres
   * Connection - Password: postgres
   * Connection - Save Password: true
   * Save

## Execute Queries via PSQL

1.  Exec into container
    - `docker exec -it database psql -U postgres`
2.  Connect to database
    - `\c postgres`
3.  Execute Command
    - `SELECT * FROM users`

## Remove

`docker compose down`
