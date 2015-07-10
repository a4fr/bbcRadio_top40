# bbc_top40
BBC radio has a program that play requested listener musics and release top 40 chart from most requested single musics. this chart has available in [BBC Radio - UK Top 40](http://www.bbc.co.uk/radio1/chart/singles). My favorite musics almost in this chart. This app has 3 parts:

1. bbc_top40_robot

2. mp3skull_robot

3. web_interface



bbc_top40_robot
---------------
Robot extract data from BBC Radio website, save datas on database (in this version on mysql) and save single music image cover in **images** directory. Also can save data as JSON file. This robot written with **python**.

mp3skull_robot
--------------
Robot after getting **artist name** and **music title** from user can search in [mp3skull](http://mp3skull.com), find best quantity and original music (not remix if exist) then download it. This robot cat help you to make a repository for download music. This robot also written with **python**.

web_interface
-------------
This part written with **php** for create a music website that show top 40 music. Because of **bbc_top40_robot** and saved data on database, website can show progression chart of every single musics (if data exist) and so on.
