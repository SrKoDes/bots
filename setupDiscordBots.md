# Documentation for Adding and Hosting Discord Bot


## *Setting Up the Code (utilizing the terminal)*

Create a directory to host the code. If the code exists in github go to the directory and run `git clone https://github.com/user-name/repo-name`.

Create a virtual environment. This will allow you to download packages without affecting your native environment’s software. Run `python3 -m venv venv`. Activate the virtual environment using `source venv/bin/activate`. 

Now we need to install all the required packages/libraries/modules for the code to run successfully. Run `pip3 -r requirements.txt`. 

## *Setting up the Application and Bot*

Next run `touch token.txt`. This will be the file that will hold the discord application’s bot’s token. Go to `https://discord.com/developers/applications`, and create an application. Name the application and select `Bot` from the sidebar. Reveal the token, copy and place it in the `token.txt`. Enable `SERVER MEMBERS INTENT`. 

`https://discord.com/api/oauth2/authorize?client_id=CLIENT_ID&permissions=0&scope=bot`: Replace the `CLIENT ID` in the URL with the Application ID in the General tab. At the edited URL, invite the bot to join the selected server.

## *Finishing Touches*
	
Run the executable that initiated the bot, in this case `main.py`.

NOTE: For MacOS users, if `main.py` returns an error, it may be because you need to install certificates. Navigate to `Applications > Python 3.9 > Install Certificates.command`. Let it run and then run `main.py` again and the bot should work!
