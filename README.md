
## Notepad with SQLite application

A notepad to keep your records in a SQLite database - a learning project to study SQL queries and inheritance in Ruby

### Possibilities:

You can make records of 3 different kinds:

0.  'Memo' -- A simple string record
1.  'Link' -- A link with a comment
2.  'Task' -- A task with a deadline

All the records automatically gain the current time info.

You can open your records sorted from new to old ones. You can also filter records by their type or view some concrete record (searched by index).


## How to use the app

 1. To save your record execute in the console
    
        ruby 'main_newpost.rb'
    
     and follow instructions.

 

 1. To read your records execute in the console
    
        ruby read.rb

You can run the app with some attributes:

 - Help information:

    ruby read.rb --h

 - Read records of some @ type:

    ruby read.rb --type @

Example:

    ruby read.rb --type Memo  
    ruby read.rb --type Task  
    ruby read.rb --type Link 
    
 - Read @ number of records:

    ruby read.rb --limit @  

Example:

    ruby read.rb --limit 10  

 - Read a record with id @:

    ruby read.rb --id @

Example:

    ruby read.rb --id 8 