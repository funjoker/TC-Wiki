---
title: achievement_criteria_data
permalink: achievement_criteria_data.html
sidebar: mydoc_sidebar
tags:
  - database
  - world
keywords: 'areatrigger, tavern, database, world'
last_updated: 'March 16, 2018'
summary: This table contains the data that a player needs to obtain / complete in order to receive a given achievement.
toc: false
folder: database/world
published: true
---

## Structure

Field                       | Type         | Attributes | Key | Null | Default | Extra | Comment 
--------------------------- | ------------ | ---------- | --- | ---- | ------- | ----- | ------- 
[criteria_id](#criteria_id) | mediumint(8) | signed     | PRI | NO   | NULL    |       |
[type](#type)               | tinyint(3)   | unsigned   | PRI | NO   | 0       |       |
[value1](#value1)           | mediumint(8) | unsigned   |     | NO   | 0       |       |
[value2](#value2)           | mediumint(8) | unsigned   |     | NO   | 0       |       |
[ScriptName](#ScriptName)   | char(64)     | signed     |     | NO   |         |       |


## criteria_id
This is the ID from Achievement_Criteria.dbc.


## type

Depending on this value, it will determine how [value1](#value1) and [value2](#value2) are used.

Type | Name
---- | ----
1    | TYPE_T_CREATURE
2    | TYPE_T_PLAYER_CLASS_RACE
3    | TYPE_T_PLAYER_LESS_HEALTH
4    | TYPE_T_PLAYER_DEAD
5    | TYPE_S_AURA
6    | TYPE_S_AREA
7    | TYPE_T_AURA
8    | TYPE_VALUE
9    | TYPE_T_LEVEL
10   | TYPE_T_GENDER
11   | TYPE_SCRIPT
12   | TYPE_MAP_DIFFICULTY
13   | TYPE_MAP_PLAYER_COUNT
14   | TYPE_T_TEAM
15   | TYPE_S_DRUNK
16   | TYPE_HOLIDAY
17   | TYPE_BG_LOSS_TEAM_SCORE
18   | TYPE_INSTANCE_SCRIPT
19   | TYPE_S_EQUIPED_ITEM
20   | TYPE_MAP_ID
21   | TYPE_S_PLAYER_CLASS_RACE
22   | TYPE_NTH_BIRTHDAY
23   | TYPE_S_KNOWN_TITLE


## value1

<pre><b>*TYPE_T_CREATURE</b></pre>

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;The target here must be a valid entry from creature_template

<pre><b>*TYPE_T_PLAYER_CLASS_RACE</b></pre>
<pre><b>*TYPE_T_PLAYER_LESS_HEALTH</b></pre>
<pre><b>*TYPE_T_PLAYER_DEAD</b></pre>
<pre><b>*TYPE_S_AURA</b></pre>
<pre><b>*TYPE_S_AREA</b></pre>
<pre><b>*TYPE_T_AURA</b></pre>
<pre><b>*TYPE_VALUE</b></pre>
<pre><b>*TYPE_T_LEVEL</b></pre>
<pre><b>*TYPE_T_GENDER</b></pre>
<pre><b>*TYPE_SCRIPT</b></pre>
<pre><b>*TYPE_MAP_DIFFICULTY</b></pre>
<pre><b>*TYPE_MAP_PLAYER_COUNT</b></pre>
<pre><b>*TYPE_T_TEAM</b></pre>
<pre><b>*TYPE_S_DRUNK</b></pre>
<pre><b>*TYPE_HOLIDAY</b></pre>
<pre><b>*TYPE_BG_LOSS_TEAM_SCORE</b></pre>
<pre><b>*TYPE_INSTANCE_SCRIPT</b></pre>
<pre><b>*TYPE_S_EQUIPED_ITEM</b></pre>
<pre><b>*TYPE_MAP_ID</b></pre>
<pre><b>*TYPE_S_PLAYER_CLASS_RACE</b></pre>
<pre><b>*TYPE_NTH_BIRTHDAY</b></pre>
<pre><b>*TYPE_S_KNOWN_TITLE</b></pre>
