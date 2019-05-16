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


# Filtring

#Show all the objects in the collection (Just the 20 on the top, if you want to see the rest type "it" rigth after you put the command and it will show you the next 20)
>db.[collection_name].find()

#Skip objects from the top of the collection *Where # is the number of objects you want to skip*
>db.[collection_name].find().skip(#)


#Limitation of showing *Where # is the number of objects you want to show from the top*
>db.[collection_name].find().limit(#) 


#Counting 
>db.[collection_name].find().count()


# Sorting 

#Asending order type 1 for desending order -1 *This works with letters and numbers*
>db.[collection_name].find().sort(#)


#Remove a document in the collection
>db.[collection_name].remove({"[Attrivute_1]": "[Caracteristics]"})


# Update

#Update a document 
>db.[collection_name].update({"$set":{"[Attrivute_1]": "[Caracteristics]"}})


#Update all the matching documents
>db.[collection_name].update({"$set":{"[Attrivute_1]": "[Caracteristics]"}},{"multi":true})


