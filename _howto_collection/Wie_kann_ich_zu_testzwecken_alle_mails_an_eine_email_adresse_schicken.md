---
title: Wie kann ich zu Testzwecken alle Mails an eine eMail-Adresse schicken ?
layout: default
tags:
  - Systemkonfiguration
lang: de
---
1. Mit Rolle "Systemadministrator" anmelden
1. Fenster "System-konfigurator" öffnen
1. Nach Name "org.adempiere.user.api.IUserBL.DebugMailTo" suchen
1. Trage in Feld **Suchschlüssel** die Email-Adresse ein an die alle Mails gehen sollen
1. Starte den Server und Deinen Client neu
