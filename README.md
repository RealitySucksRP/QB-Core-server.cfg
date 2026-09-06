# QB-Core Server.cfg Beginner Guide

<p align="center">
  <a href="https://reality-sucks-rp-webstore.tebex.io/"><img src="https://img.shields.io/badge/BROWSE-REALITYSUCKSRP%20TEBEX-ff6a00?style=for-the-badge" alt="Browse RealitySucksRP Tebex Store"></a>
  <a href="https://realitysucksrp.github.io/#packages"><img src="https://img.shields.io/badge/VIEW-COMPLETE%20SERVER%20PACKAGES-111111?style=for-the-badge" alt="View RealitySucksRP server packages"></a>
  <a href="https://discord.gg/e9V3rPHySx"><img src="https://img.shields.io/badge/ASK%20ME-DISCORD-5865F2?style=for-the-badge" alt="Join RealitySucksRP Discord"></a>
</p>

> I build complete FiveM server setups using my own tested systems: shops, weapons, phones, racing, LS Customs, garages, dealerships, zombie apocalypse systems, warfare, Phantom encounters, UI and more. I configure the stack around what the server owner actually wants.

This repository is designed for new FiveM server owners who are just getting started with QB-Core and server configuration.

At first, `server.cfg` can look overwhelming. That is normal. It controls how your FiveM server starts, what resources load and how everything connects together.

## What This File Controls

- Server name and branding
- Player slots
- FiveM license key
- Database connection
- QB-Core load order
- Scripts, jobs and systems
- Voice, UI and gameplay resources

## What You Must Edit

### Server Name
```cfg
sv_hostname "INSERT SERVER NAME HERE"
```

### License Key
```cfg
sv_licenseKey "INSERT LICENSE KEY HERE"
```

### Database Password
```cfg
mysql_connection_string "mysql://root:INSERT_PASSWORD_HERE@127.0.0.1:3306/qbcore"
```

### Optional Server Password
```cfg
sv_password "INSERT PASSWORD HERE"
```

## Why Load Order Matters

Core resources should load first, systems second and addons last.

A bad load order can cause resources to fail, dependencies to be missing or the server to behave unpredictably.

Typical structure:

```cfg
ensure oxmysql
ensure qb-core

# Core systems
ensure qb-inventory
ensure qb-target

# Jobs / gameplay / custom resources
ensure your-resource
```

## Complete FiveM Servers For Sale

I love making scripts and running wild in GTA, but I also enjoy building complete servers. I use tested RealitySucksRP systems and configure the build around the owner's gameplay, framework, economy, theme and direction.

- **QBCore Shell — $500**
- **Zombie Server — $700**
- **Full RP Server — $850**
- **30 days of Discord setup/support included**

**Website:** https://realitysucksrp.github.io/

**Tebex:** https://reality-sucks-rp-webstore.tebex.io/

**Discord:** https://discord.gg/e9V3rPHySx

## Final Note

Use this repository as a learning tool and starting point. Make small changes, test often and keep backups before changing a live server.

---

Made by RealitySucksRP.