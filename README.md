# mongo_tutorial
Basic Mongo Tutorial

> = Command line
# = Comment


#Show the created data bases
>Show dbs


#Switches to use the database and creates it if doesn't exist
>Use [DATABASE]


#Create a variable
>[Name] = {"[Attrivute_1]": "[Caracteristics]", "[Attrivute_2]": "[Caracteristics]"}


#Create a collection
>db.[collection_name].insert()


#Show Collections
> db.getCollectionNames()


#Insert a variable into the collection
>db.[collection_name].insert({"[Attrivute_1]": "[Caracteristics]", "[Attrivute_2]": "[Caracteristics]"})


#Show vaiables in the collection
>db.[collection_name].find()


#Remove a variable in the collection
db.[collection_name].remove({"[Attrivute_1]": "[Caracteristics]"})
