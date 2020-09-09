# Cinema
## Choose useful attributes and relations


The STAR-MOVIES company operates a cinema chain with several cinemas (Name,
Address... ). Each cinema can have several halls where the films are shown. The seating plan of each hall should be recorded; a row and a seat must be indicated for each seat. A box should be managed like a row.
It must be possible to create a seating plan. Of course, several films can be shown per room on one day. In order to be able to determine which seats are available for a performance, each ticket purchase must be noted. Each ticket should show: cinema, hall, film title, date, starting time, serial number within the screening, row, seat, price.
Provision must be made for pricing: Each row of a hall has a standard price, but for certain performances the row prices can be set individually. For information purposes, the actors should be recorded with their personal data (surname, first name, nationality, date of birth, date of death, comments, ... ) and it should be possible to tell which actors have acted in which films.
The analogous statements should also be possible for directors, whereby it can be assumed that there is only one director for a film. However, it is possible that the director also plays a part in a film.
The other data of a film include: Title, type (thriller, western, youth film, ... ), year of production, country, language, duration, distribution, etc.

Create a ERD and a Relation Model for this example

# Finish

Cinema (CID: int, Name: varchar, Address: varchar, Halls: int)

Hall (HID: int, Rows: int, Seats: int)

Seat Plan (ID: int, SID)

Seat (SID: int)

Box (RowID: int)

Ticket (TID: int, FName, Price, HID, SID, RowID)

Film (FID: int, FName: varchar)

Price (Price: double)

Actor (AID: int, LName: varchar, Nation: varchar, BD: date, DD: date, Comment: varchar)

Director (DName: int)

![Photo](photo.jpg)