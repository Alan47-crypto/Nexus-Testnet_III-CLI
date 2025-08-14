# Nexus Testnet III CLI Contribution Guide
## Step 1: Install the Nexus Software 💻
First, let's get the main tool installed on your computer.

Open your terminal.

Copy and paste the following command, then press Enter. This will automatically download and set up the Nexus command-line tool for you.

```Bash

curl https://cli.nexus.xyz/ | sh
```
![Installation screen](https://private-user-images.githubusercontent.com/78281099/478248751-b721f8e5-3987-48cf-9a30-2adb158046b1.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTUyMTM3MDQsIm5iZiI6MTc1NTIxMzQwNCwicGF0aCI6Ii83ODI4MTA5OS80NzgyNDg3NTEtYjcyMWY4ZTUtMzk4Ny00OGNmLTlhMzAtMmFkYjE1ODA0NmIxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MTQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODE0VDIzMTY0NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTJjZTlmZGFhMWQ1NDEwZjYxMTVmZDg3OWFkYzEzNzRjNmU1MzYwYWU5MjllYmU2ZmQxMmUyNTdmNzQzN2M3NDAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.r-g10oBMGA2S08EvXn9hQTk1QXa_cTvOFDjShxguSiM)


Once it's done, refresh your terminal so it recognizes the new commands. You can either close and reopen the terminal window or run a command:

```bash
source ~/.bashrc
```

## Step 2: Your First-Time Setup 🚀
When you run the software for the first time, you'll go through a quick setup process. You'll be asked to:

Accept the Terms of Use.

Choose how you want to contribute. You have two great options:

🔗 Link to a Nexus Account (Recommended):
This is the best option if you want to get rewarded for your contributions. You'll be able to earn NEX Points, track your rank on the leaderboard, and manage all your devices (nodes) from one simple dashboard. To get started, create an account at app.nexus.xyz and follow the instructions in the terminal.


🥷 Anonymous Proving:
If you prefer privacy, you can contribute without linking an account. Your work still helps the network, but you won't earn points or show up on the leaderboard.

## Step 3: Install screen (A One-Time Step) 🛠️
To keep your node running 24/7, we'll use a tool called screen. First, we need to make sure it's installed. This is a one-time setup.

Run this command to update your package lists and install screen.

```Bash

sudo apt update && sudo apt install screen -y
```

## Step 4: Start Your Node to Run 24/7 (Using screen) ✨
Now that screen is installed, let's use it to start your node so it stays online.

Create a New Screen Session: In your terminal, type the following command to create a session named nexus.

```Bash

screen -S nexus
```
Your terminal window will clear and you are now "inside" the new session.

- This step requires Node ID, open your browser and go to Nexus dashboard [HERE](https://app.nexus.xyz/)
   - Sign up (for new user) or login (existing users)
   - Click on Nodes then add CLI Node
   - Copy your Node ID and go back to your terminal
 
![Dashboard SS](https://private-user-images.githubusercontent.com/78281099/478249158-e8627df0-83f4-4dbb-a244-7414046822ce.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTUyMTM3MDQsIm5iZiI6MTc1NTIxMzQwNCwicGF0aCI6Ii83ODI4MTA5OS80NzgyNDkxNTgtZTg2MjdkZjAtODNmNC00ZGJiLWEyNDQtNzQxNDA0NjgyMmNlLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MTQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODE0VDIzMTY0NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTZkYmE2MmJlMjZiYzQ2Njg5NDdiYWNhYTU2NGI3Mjk1MTdlZGYyMjI1MzUxYWY1MmE1ZmJiYTY1ZmRhNzdjMzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.Ph4oKraI_qZEhOLaSYvbylxA2GNtwng8TyHQ_LKLLzQ)

![NODE ID SS](https://private-user-images.githubusercontent.com/78281099/478249325-3a107aa2-61ee-43f5-b709-f2f0797f4616.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTUyMTM3MDQsIm5iZiI6MTc1NTIxMzQwNCwicGF0aCI6Ii83ODI4MTA5OS80NzgyNDkzMjUtM2ExMDdhYTItNjFlZS00M2Y1LWI3MDktZjJmMDc5N2Y0NjE2LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MTQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODE0VDIzMTY0NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWE4OGM0YTU3NmEzYjNkOGMzODA2NTE0YzU0MDc4ZDE4NzMyYWE3OTgzZDJjZmNiNDkwZTgxMTMwYzBkYWZiNzkmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.89wVeBxzr-HEzgCr6LGAiRsOt3Eh47KgWR__QNCHwtg)


- Start your node with this command.
Replace `<your-node-id>` with your actual Node ID you copied from node dashboard.

```Bash

nexus-network start --node-id <your-node-id>
```
![Prover NODE SS](https://private-user-images.githubusercontent.com/78281099/478248750-07e3b26f-e212-4bc1-8691-4ff27e3e1e32.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTUyMTM3MDQsIm5iZiI6MTc1NTIxMzQwNCwicGF0aCI6Ii83ODI4MTA5OS80NzgyNDg3NTAtMDdlM2IyNmYtZTIxMi00YmMxLTg2OTEtNGZmMjdlM2UxZTMyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MTQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODE0VDIzMTY0NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTAwOWRkYzQ3NjQ4NjhlNmNmOTQwY2VmY2NlZTc5MThlZDIwZGE3OTM2M2IwOWZiNTcxZTBmZTU0MGI0NTZlMDMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.rhAcuj2bJWWW5x7givNro5hYYxVKWuiEbjfuPv8B6rU)


Detach from the Session: Once your node is running, you can safely detach from the session, leaving it running in the background. To do this, press `Ctrl+A` on your keyboard, and then press `D`.

That's it! Your node is now running, and you can close your main terminal window.

## Step 5: Managing Your Session & Account 🔑
How to Check on Your Node
When you want to check the status of your running node, just reconnect to your server and use this command to "re-attach" to your nexus session:

```Bash

screen -r nexus
```
You'll see the live output of your node. When you're done, just detach again `Ctrl+A`, then `D`.

![Screen Detach](https://private-user-images.githubusercontent.com/78281099/478251850-f9627e13-d202-42b4-b72f-55862897df40.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NTUyMTQxODcsIm5iZiI6MTc1NTIxMzg4NywicGF0aCI6Ii83ODI4MTA5OS80NzgyNTE4NTAtZjk2MjdlMTMtZDIwMi00MmI0LWI3MmYtNTU4NjI4OTdkZjQwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNTA4MTQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjUwODE0VDIzMjQ0N1omWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTIwYTAwOTQ1MDc4N2ZkNmY4NmJjMjc2YWJhOTM0OTcwMDNjMzgyODc4YzIwOWQ1OWQ1MzJkNjA1MjFjNGNhNDQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0In0.T8rOMlBjXQe5NOLsQg20_v8UQFm95JK2h0Tmhp2lcQw)
