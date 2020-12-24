# FriendSystem
[![](https://poggit.pmmp.io/shield.state/Friends)](https://poggit.pmmp.io/p/Friends)

A plugin for PocketMine-MP.
Now your players can add they friend each other!
Easy and useful.

# default config.yml
friend-tp: false

# default data.yml
friends: []
invites:
  example: []

# default messages.yml
friendcommand:
  name: "friend"
  description: "Manage your friends"
  aliases:
  - f
  usage: "§cUsage: §7/friend help"
  error-use-ingame: "§c> Use this command in game."
  permission: false

  subcommands:
    help:
      name: "help"
      aliases:
      - h
      success1: "§e> Friend Help"
      success2: "§a> %0 - %1"
    invite:
      name: "invite"
      description: "Send friend requests"
      usage: "§cUsage: §7/friend invite <player>"
      aliases:
      - i
      error-already-friend: "§c> This player is already your friend."
      error-already-invited: "§c> You are already invited this player."
      success1: "§a> Player %0 successfully invited."
      success2: "§a> Player %0 sent friend request to you."
    list:
      name: "list"
      description: "Your friend list"
      usage: "§cUsage: §7/friend list"
      aliases:
      - l
      error-no-friends: "§c> You have no friends. §7*sad*"
      success: "§a> Your friends: %0"
    remove:
      name: "remove"
      description: "Removes friend"
      usage: "§cUsage: §7/friend remove <player>"
      aliases:
      - r
      error-not-friend: "§c> Player %0 is not your friend."
      success1: "§a> Player %0 removed from your friend list."
      success2: "§a> Player %0 removed you from his friend list."
    accept:
      name: "accept"
      description: "Accepts friend request"
      usage: "§cUsage: §7/friend accept <player>"
      aliases:
      - a
      error-not-invited: "§c> This player is not invited you."
      success1: "§a> You are accepted %0's friend request."
      success2: "§a> %0 accepted your friend request."
    deny:
      name: "deny"
      description: "Refuses friend request"
      usage: "§cUsage: §7/friend deny <player>"
      aliases:
      - d
      error-not-invited: "§c> This player is not invited you."
      success1: "§a> You are denied %0's friend request."
      success2: "§a> %0 denied your friend request."
    chat:
      name: "chat"
      description: "Sends private message to friends"
      usage: "§cUsage: §7/friend chat <player> <message>"
      aliases:
      - c
      error-not-friend: "§c> Player %0 is not your friend."
      success1: "§a> You to %0: %1"
      success2: "§a> %0 to You: %1"
    teleport:
      name: "teleport"
      description: "Lets you teleport friend"
      usage: "§cUsage: §7/friend teleport <player>"
      aliases:
      - tp
      error-not-friend: "§c> Player %0 is not your friend."
      success1: "§a> Teleported friend named %0."
      success2: "§a> Your friend named %0 teleported to you."
    cancelinvite:
      name: "cancelinvite"
      description: "Cancel your friend request"
      usage: "§cUsage: §7/friend cancelinvite <player>"
      aliases: []
      error-not-invited: "§c> You are not invited this player."
      success: "§a> You are cancelled friend request."
    invites:
      name: "invites"
      description: "Shows your friend requests"
      usage: "§cUsage: §7/friend invites"
      aliases: []
      error-not-invited: "§c> You have no friend requests."
      success: "§a> Your friend requests: %0"
friend-joined: "§7[§a+§7] §aYour friend §b%0 §ajoined to server."
friend-left: "§7[§c-§7] §cYour friend §b%0 §cleft from server."
