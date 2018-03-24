---
title: access_requirement
permalink: access_requirement.html
sidebar: mydoc_sidebar
tags:
  - database
  - world
keywords: 'areatrigger, tavern, database, world'
last_updated: 'March 16, 2018'
summary: This table contains the access requirements to enter an instance.
toc: false
folder: database/world
published: true
---


## Structure

Field                                           | Type         | Attributes | Key | Null | Default | Extra | Comment 
----------------------------------------------- | ------------ | ---------- | --- | ---- | ------- | ----- | ------- 
[mapId](#mapId)                                 | mediumint(8) | unsigned   | PRI | NO   | NULL    |       |
[difficulty](#difficulty)                       | tinyint(3)   | unsigned   | PRI | NO   | 0       |       |
[level_min](#level_min)                         | tinyint(3)   | unsigned   |     | NO   | 0       |       |
[level_max](#level_max)                         | tinyint(3)   | unsigned   |     | NO   | 0       |       |
[item_level](#item_level)                       | smallint(5)  | unsigned   |     | NO   | 0       |       |
[item](#item)                                   | mediumint(8) | unsigned   |     | NO   | 0       |       |
[item2](#item2)                                 | mediumint(8) | unsigned   |     | NO   | 0       |       |
[quest_done_A](#quest_done_A)                   | mediumint(8) | unsigned   |     | NO   | 0       |       |
[quest_done_H](#quest_done_H)                   | mediumint(8) | unsigned   |     | NO   | 0       |       |
[completed_achievement](#completed_achievement) | mediumint(8) | unsigned   |     | NO   | 0       |       |
[quest_failed_text](#quest_failed_text)         | text         | signed     |     | NO   | NULL    |       |
[comment](#comment)                             | text         | signed     |     | NO   | NULL    |       |


## mapId
This is the [access_id](instance_template.html#acess_id) field from the [instance_template](instance_template.html) table. It is an arbitrary number that merely links the requirements to an [instance_template](instance_template.html), or [areatrigger_teleport](areatrigger_teleport.html).


## difficulty
5 man dungeons - 0 for normal, 1 for heroic, 2 for epic (not used yet)

10 man dungeons - 0 for normal, 2 for heroic

25 man dungeons - 1 for normal, 3 for heroic


## level_min
The minimum level that you must be in order to enter the instance.


## level_max
The maximum level that you can be in order to enter the instance.


## item_level
The at least required item level for a instance.

All WotLK Heroics require at least an average item level of 180.
Trial of the Champion, Pit of Saron, and the Forge of Souls require an average item level of 200.
Halls of Reflection requires an average item level of 219.


## item
An item that you must have in your inventory to enter the instance. This item can not be in the bank.


## item2
A second item that you must have in your inventory. This item can not be in the bank.


## quest_done_A
A quest that you must have completed. This field is only for alliance.


## quest_done_H
A quest that you must have completed. This field is only for horde.


## completed_achievement
An achievement that must be completed by the player to enter an instance.


## quest_failed_text
The text that is shown if you try and enter the instance without having completed the quest.


## comment
This field is for any comment you want to make about the requirements. It is arbitrary text.


{% include links.html %}
