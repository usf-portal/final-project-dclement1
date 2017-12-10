# Design

    To create a relational database, one must first develop some manner of categorizing the data such a manner where the different categories relate to each other in some fashion. These different categories are called tables, or models, and are at their essence, simply different groupings of columns from a spreadsheet.

    Designing the database for this particular dataset initially seemed fairly straightforward, however required several attempts to fine tune and refine, before I was satisfied with it. Ultimately it was the design that proved the largest challenge with this project. The database would be created using a free program entitled, MySQL Workbench. This is a program which allows you to design a SQL database, graphically, rather than purely in code. This allows someone with only a rudimentary knowledge of SQL language to create and design database. The decision was made to make five main tables: Mission, Location, Target, Ordinance, Units. These five tables are joined together via intermediary tables which serve simply as place holders for ID numbers which relate each table to the other. In addition, the Ordinance table was related to the target table, so that it would be possible to query the database for things such as the amount of ordinance dropped on a particular target. Similar relations were formed between the Units table and the Ordinance table. in addition, the Mission table has had relationships connected to all of the other tables. An image of the graphical representation of the schema, as designed in MySQL Workbench is displayed below.

    I have also created two views, which are a way of designing a query, and then saving it, so that in the future, you can simply use the view, as opposed to writing the entire code for the view.
    The first view I created was a view which will display information about units and the ordinance they used at specific target locations. This would be useful if you wanted to quickly find out statistics about ordinance dropped on targets.
    The second view I created produces the number of missions a specific unit went on. This could be used as reference in research on specific units. It could also be used as a way to realize new and interesting insights which would be difficult to gain through traditional humanities efforts.

[Final Version of the Schema](imgs/included/Scheema_Design3.png)


    Also included is the MySQL Workbook file, which contains the schema design.
[Workbook file](files/WWII_Bombing_DB_Final.mwb).
