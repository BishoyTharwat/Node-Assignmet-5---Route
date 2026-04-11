Assignment 5
# Part 1: ERD Diagram

## Entities:

### 1- musician : 
- MusicianId (Primary Key) 
- Name 
- Street 
- City 
- Phone

### 2- instrument : 
- InstrumentName (Primary Key) 
- MusicalKey

### 3- album : 
- AlbumId (Primary Key) 
- AlbumTitle 
- CopyrightDate

### 4- song : 
- SongTitle (Primary Key) 
- Author

### 5- MusicianInstrument : 
- MusicianId 
- InstrumentName

### 6- MusicianSongs : 
- MusicianId 
- SongTitle

## Relations:
-  musician ~ instruments : M-M
- album ~ song : 1-M
- song - musician : M-M
- musician ~ album : 1-M


----

# Part 2: Design a schema (Mapping)

## Entities:
### 1- User
 - u_id (pk) 
 - email 
 - role 
 - password 
 - fName 
 - lName


### 2- Product
- prod_id (pk) 
- name - stock 
- isDeleted 
- price 
- u_id (Fk)


### 3- User_Phone : 
- u_id, phone (Composite pk) 
- u_id (Fk) 
- phone 