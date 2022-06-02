## StarkNet, Node Installation Guide English Translation.

# First we create an Alchemy account.

We will use nodes provided by the Alchemy service to run Starknet, so sign up at [alchemy.com](https://www.alchemy.com/) and we will create endpoints in your personal account.

# Images in sequence:

![image](https://user-images.githubusercontent.com/101149671/171650488-9846b8e5-d76d-43a7-a256-402cba2e0f8a.png)

![image](https://user-images.githubusercontent.com/101149671/171650517-7b22a87e-fff5-4704-b38b-1464f82e83f2.png)

![image](https://user-images.githubusercontent.com/101149671/171650593-c63e40b7-71c3-4c14-8a69-daf26a066677.png)

![image](https://user-images.githubusercontent.com/101149671/171650619-a0527993-19ec-4ce0-a674-033b68da1cea.png)

![image](https://user-images.githubusercontent.com/101149671/171650653-8eb80d02-d369-4602-9770-cd0d17fa8a06.png)


Create the account as I have shown in the images and copy the address.

# SETUP

```
ALCHEMY=YOUR_ALCHEMY_HTTP_ADDRESS
echo 'export ALCHEMY='$ALCHEMY >> $HOME/.bash_profile
```

YOUR_ALCHEMY_HTTP_ADDRESS enter the address we just copied from alchemy.

# Script for quick installation:

```
wget -O starknet.sh https://api.nodes.guru/starknet.sh && chmod +x starknet.sh && ./starknet.sh
```

# To follow the logs:

```
journalctl -u starknetd -f
```

# To restart the node:
```
systemctl restart starknetd
```

# To delete a node:
```
systemctl stop starknetd
systemctl disable starknetd
rm -rf ~/pathfinder/
rm -rf /etc/systemd/system/starknetd.service
rm -rf /usr/local/bin/pathfinder
```

# That's all the procedures, thank you.
```
https://t.me/RuesAnnouncement
https://t.me/RuesChat
https://t.me/RuesNode
https://t.me/RuesNodeChat
https://forum.rues.info/
```



















