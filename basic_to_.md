# Mongo tutorial
From basic to ...


"#" = Comment


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


#Insert a document into the collection
>db.[collection_name].insert({"[Attrivute_1]": "[Caracteristics]", "[Attrivute_2]": "[Caracteristics]"})


#Show all the collections
>db.[collection_name].find()


#Remove a document in the collection
>db.[collection_name].remove({"[Attrivute_1]": "[Caracteristics]"})


#Update a document 
>db.[collection_name].update({"$set":{"[Attrivute_1]": "[Caracteristics]"}})


#Update all the matching documents
>db.[collection_name].update({"$set":{"[Attrivute_1]": "[Caracteristics]"}},{"multi":true})


