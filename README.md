📘 Beginner Guide

This repository is designed for new FiveM server owners who are just getting started with QB-Core and server configuration.

At first, this file may look overwhelming — that’s normal.

You are seeing a full server.cfg template, which controls how your FiveM server starts, what resources load, and how everything connects together.

🧠 Important Message for Beginners

If this is your first time setting up a server:

Don’t panic if it feels confusing.

You do NOT need to understand everything at once.

Just follow the structure step-by-step and it will start to make sense over time.

Most people learn this gradually by:

making small changes
testing the server
fixing errors as they appear
⚙️ What This File Does

The server.cfg controls:

Server name and branding
Player limit (slots)
License key connection to FiveM
Database (MySQL / MariaDB)
Core framework loading order (QB-Core)
All scripts, jobs, and systems
Voice, UI, and gameplay features
📌 What You MUST Edit

Before starting your server, you must change:

Server Name
sv_hostname "INSERT SERVER NAME HERE"
License Key
sv_licenseKey "INSERT LICENSE KEY HERE"
Database Password
mysql://root:INSERT_PASSWORD_HERE@127.0.0.1:3306/qbcore
Optional Password
sv_password "INSERT PASSWORD HERE"
⚠️ Why Structure Matters

The order of resources is very important.

Core resources must load first (qb-core, oxmysql)
Systems load second (inventory, jobs, housing)
Addons and extras load last

If the order is wrong, your server may:

crash
fail to start
or have missing features
🚀 Final Note

This file is meant to be a learning tool and starting point.

Take your time, make changes slowly, and test often.

Once you understand this structure, you’ll be able to build and customize full FiveM servers with confidence.
