[![svgviewer-png-output](https://github.com/user-attachments/assets/8d8e02a0-13c7-4c13-8bbf-91ffd87b02dc)](https://penguinmod.com)
[![svgviewer-png-output (1)](https://github.com/user-attachments/assets/68934725-8189-47ba-99ef-44ec0c51ee6b)](https://theshovel.rocks)

# Accord

Accord is a very basic and anonymous Discord-like chat room, built with PenguinMod! <br>
Originally built for TheShovel.Rocks <br>
![image](https://github.com/user-attachments/assets/ffa3e72b-3a3b-4294-a9ca-6f7ef8027822)

Check it out at [>chat.theshovel.rocks<](https://chat.theshovel.rocks)

### Host your own!

It's quite easy to host your own Accord channel! <br><br>
If you don't want to rely on my websocket server you can do this: <br>
You need to host a [>websocket-server<](https://github.com/WorldSprites/websocket-server) from the WorldSprites repository. It's a basic Node based server, you can just run it with the latest version of Node and it should work.<br><br>
You dont have to do this though! You can just use my server, and change the channel name in the config file!

#### Configuration

Most of the configuration is found in the `channel.json` file. There you can change the server to your own, along with the name that is displayed for it in the app, add rooms, set the default room and list the profile pictures.<br><br>
You can also define what themes can be selected by adding or removing entries inside `themes.json`.

#### Images

All image assets are inside the `images` folder. There you can replace the welcome screen, or add the images for your pre-defined profile pictures, inside the `pfps` folder.

#### Static rooms

Static rooms are rooms that can only display messages inside a pre-defined json file. This can be used to add announcements rooms or other stuff like that. You can make a static room by setting `static` to true inside the definition of the room inside the `channel.json` file.<br>
You can set the values inside these channels by making a json file in the root directory with the scheme `ROOMNAME-static.json`. Look at the examples to see how to format the messages. Static rooms also support different embed types (images, GitHub links, Youtube links).

### Modifying the client

Generally, I don't think you would need to do this, but if you want to mess around, you can run `start-server.sh`, or start a localhost server on port 8000 in the root directory of the repo, and then open the `accordapp.pmp` file in [>PenguinMod<](https://theshovel.rocks/stable-penguinmod/build/editor.html).

### Moderation apis

By default, Accord uses [>profanity.dev<](https://www.profanity.dev/) for it's username and message filtering. This can be changed inside the `channel.json` file.
