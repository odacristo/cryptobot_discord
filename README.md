<html>
<body style="font-family: Consolas, monospace; font-size:14pt;">
<b>Discord CryptoBot installation instructions</b>
<br/> ────────────────────────────────────────────────────
<br/>
<br/> A beautiful discord bot that allows you to track your favourite masternodes balances and performances.
<br/>
<br/> <b>0. Requirements</b>
<br/>
<br/> In order to run this program the following python3 and the following libraries need to be installed:
<br/> &nbsp; &nbsp; $sudo apt-get install python3-pip python3-yaml
<br/> &nbsp; &nbsp; $sudo pip3 install -U discord.py
<br/> &nbsp; &nbsp; $sudo pip3 install coinmarketcap
<br/>
<br/> <b>1. Copying the necessary files</b>
<br/>
<br/> &nbsp; &nbsp; $mkdir -p /opt/cryptobot_discord/
<br/> &nbsp; &nbsp; $cd /opt/cryptobot_discord/
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/cryptobot_discord.py
<br/>
<br/> -- These are configuration examples, you need to customize them --
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/config/smartcash_bot.yml
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/config/tokugawa_bot.yml
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/config/loki_bot.yml
<br/>
<br/> <b>2. Setting your configuration file</b>
<br/> 
<br/> Edit the configuration file and modify as needed; coin parameters, masternodes addresses, etc...
<br/> If the coin explorer base url is not known by you contact the coin developer.
<br/> In the Discord section add your API key (check how to create a key <a href="https://discordpy.readthedocs.io/en/rewrite/discord.html">here</a>).
<br/>
<br/> <b>3. Executing the script</b>
<br/> &nbsp; &nbsp; $python3 cryptobot_discord.py /your_path/your_configuration.yml &
<br/>
<br/> <b>4. Optional starting the bot automatically at boot</b>
<br/> If you want to automatically start yours bots at boot consider to add them to systemctl.
<br/> You can check the predefine bot services available in: https://github.com/Lyndros/cryptobot_discord/tree/master/service/.
<br/> Please before enabling edit the file location as needed.
<br/>
<br/> i.e: Adding tokugawa bot service,
<br/> &nbsp; &nbsp; $cd /etc/systemd/system/
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/service/tokugawa_bot.service
<br/> &nbsp; &nbsp; $systemctl enable tokugawa_bot.service
<br/> 
<br/> i.e: Adding smartcash bot service,
<br/> &nbsp; &nbsp; $cd /etc/systemd/system/
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/service/smartcash_bot.service
<br/> &nbsp; &nbsp; $systemctl enable smartcash_bot.service
<br/>
<br/> i.e: Adding loki bot service,
<br/> &nbsp; &nbsp; $cd /etc/systemd/system/
<br/> &nbsp; &nbsp; $wget https://raw.githubusercontent.com/Lyndros/cryptobot_discord/master/service/loki_bot.service
<br/> &nbsp; &nbsp; $systemctl enable loki_bot.service
<br/>
<br/> <b>5. Chatting withs your bot</b>
<br/> To see a list of available bot commands, open a chat with your bot and type "/bot ayuda"
<br/>
<br/> <b>6. Donations</b>
<br/> If you want o support this repository I accept donations even 1 TOK is always welcome :-)!
<br/> &nbsp; &nbsp;> <b>ethereum address:</b> <i>0x44F102616C8e19fF3FED10c0b05B3d23595211ce</i>
<br/> &nbsp; &nbsp;> <b>tokugawa address:</b> <i>TjrQBaaCPoVW9mPAZHPfVx9JJCq7yZ7QnA</i>
<br/>
<br/> For any questions feel free to contact me at <i>lyndros@hotmail.com</i>
</body>
</html>
