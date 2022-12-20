# EdgeGamers Customized Basechat
A derivation of the original [basechat included in SourceMod](https://github.com/alliedmodders/sourcemod/blob/master/plugins/basechat.sp).

# Installation
1. Delete (or move to disabled/) the original sourcemod basechat.smx file from your `plugins` folder.
2. Compile and move the `basechat.smx` file into the `plugins` folder.
3. Combine the `Chat to admins-admin` and `Chat to admins-source` phrases from `addons/sourcemod/translations` into your `common.phrases.txt` file (or copy the file completely).

## Features
- Includes UID of players when they contact admins.
- Overhauls team/all channels to be consistent between both.
- Adds "r" (respond) alias to allow admins to easily respond to whomever they most recently messaged.
  - Example:
  - sm_psay #576 Hello
  - sm_psay r How are you? (Would send to #576)
  - @@MSWS wassup
  - @@r sup (would also send to MSWS)
- Logs all messages (chat, psay, etc.)

## Differences
- Removes the `sm_hsay` command. (Did not work on CS:GO)
- Admin chat is now accessible to non-admins through both team and all chat.
- Uses `Chat to admins-admin` and `Chat to admins-source` accordingly instead of the plain `Chat to admins`.