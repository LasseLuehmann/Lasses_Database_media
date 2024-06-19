# Lasses_Database_media
This repo contains the code for creating and interacting with my database

## Mission Statement:
This program takes care of all of your films and games in order to keep track of it

## Mission Objective:
- get a overview of all games and films
- be able to easily select them by certain phrases

## Preperation
1. Inside the `src` package are two sql modules
    - `tables.sql`
    - `insertions.sql`
```bash
cd <absolute_path>/Lasses_Database_media/src
psql -U postgres
```
2. Run those in your psql shell to create the database structure
```sql
\i tables.sql
\i insertions.sql
```
3. to properly use the program I recommend to open your terminal as full screen

### Insertions into the media table
Now you are able to add your media into the media table.
In order to do so follow the describtion.
```bash
cd <absolute_path>/Lasses_Database_media
python3 -m src/main
# The menu will apear now you have to select 4 for insertion
Enter name: # <Enter the name of the media>
(1, 'Game')
(2, 'Film')
Take the related number! 
Enter type_id: # <Enter the number wich matches your media>
(1, 'Documentation')
(2, 'Action')
(3, 'Science Fiction')
(4, 'Horror')
(5, 'Fantisy')
(6, 'Crime')
(7, 'Comedi')
(8, 'Animation')
(9, 'Sandbox')
(10, 'ActionRPG')
(11, 'RPG')
(12, 'Survival')
(13, 'Strategie')
(14, 'Shooter')
(15, 'Stealth Action')
(16, 'Rennen')
(17, 'Fighter')
(18, 'Hack&Slay')
(19, 'Jump&Run')
Take the related number!
Enter genre_id: # <Enter the number wich matches your media denre>
Enter publisher(optional): # <Enter the publisher>
Enter publishing_date YYYY/MM/DD(optional): # <Enter the publishing year>
Enter fsk: # <Enter the age restriction> 
Enter carrier_type: # <Enter the type of carrier>
('PC',)
('PSP',)
('Xbox360',)
('PS4',)
('DVDply',)
Take the matching platform!
Enter platform: # <Enter the the platform name>
```

## How to run:
1. When the program starts you will see a menu with related numbers and you'll be prompt to take a choice.
2. Depending on your choice you will access either another menu or one of the whole tables.


### NOTE
It is not finished yet
Further ideas are:
- finishing the select by publisher and by type of media
- Add an update option

