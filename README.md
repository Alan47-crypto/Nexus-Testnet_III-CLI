# Nexus Testnet III CLI Contribution Guide
## Step 1: Install the Nexus Software 💻
First, let's get the main tool installed on your computer.

Open your terminal.

Copy and paste the following command, then press Enter. This will automatically download and set up the Nexus command-line tool for you.

```Bash

curl https://cli.nexus.xyz/ | sh
```
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

- Start your node this command.
Replace `<your-node-id>` with your actual Node ID you copied from node dashboard.

```Bash

nexus-network start --node-id <your-node-id>
```
Detach from the Session: Once your node is running, you can safely detach from the session, leaving it running in the background. To do this, press `Ctrl+A` on your keyboard, and then press `D`.

That's it! Your node is now running, and you can close your main terminal window.

## Step 5: Managing Your Session & Account 🔑
How to Check on Your Node
When you want to check the status of your running node, just reconnect to your server and use this command to "re-attach" to your nexus session:

```Bash

screen -r nexus
```
You'll see the live output of your node. When you're done, just detach again `Ctrl+A`, then `D`.

