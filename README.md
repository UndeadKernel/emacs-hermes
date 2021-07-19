# emacs-hermes

emacs-hermes is an Emacs interface to remotely control Emacs through messages.

## What is it
In ancient Greek mythology, Hermes is knows as the herald of the gods: he who's responsible for transporting and delivering messages. This package provides a mechanism to receive messages through different communication channels that may trigger Emacs functions. With emacs-hermes, you should be able to configure things such as:
+ Adding a message to an org file by sending an email
+ Retrieving information below an org headline by asking a Telegram bot
+ Triggering a user-defined elisp function after polling certain content from a website

emacs-hermes is at an early development stage. This repository will be updated as development moves forward. Does this project sound interesting to you? Feel free to submit issues with ideas or suggestions.

## Messaging Systems
emacs-hermes is meant to be able to receive messages from different sources. Development efforts are currently focused on creating an interface to communicate with a Telegram bot. Other interfaces will follow.

### Telegram Bot
A telegram bot may be used to contact emacs-hermes. A telegram bot (server) needs to be running and connected to the Telegram network. Afterwards, you should be able to contact this bot, authenticate, and issue messages for emacs-hermes to process.
You decide how to process the messages. emacs-hermes provides the facilities to program how emacs reacts to different messages. For example, send a text message to the Telegram bot with something like:

> ol Shopping Apples Carrots Nuts

and emacs-hermes should be able to add to the `Shopping` org headline the elements `Apples`, `Carrots` and `Nuts`. You decide how emacs-hermes reacts to different messages. Default actions shall be provided. 
