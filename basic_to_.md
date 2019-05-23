# Mongo tutorial
From basic to ...

# Essential

#Switches to use the database and creates it if doesn't exist
>Use [DATABASE]


#Create a variable
>[Name] = {"[Attrivute_1]": "[Caracteristics]", "[Attrivute_2]": "[Caracteristics]"}

# Starting

#Show the created data bases
>Show dbs

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


#Show just the desired attributes
>db.[collection_name].find({"[Attrivute_1] : "[Caracteristics]"},{ [Attrivute_#]: true, [Attrivute_#]: true) 



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


# Operators

$gt       (Greater than)


$gte      (Greater than or equal to)


$ne       (Not equal)


$lt       (less than)


$lte      (less than or equal to)


$max      (Updates if new value is greater than current or inserts if empty)


$min      (Updates if new value is less than current or inserts if empty)


$mul      (Multiplies current field value by specified value. If empty, it inserts 0)


$sum      (Sums)


$avg      (Average)


$match    (Passes documents to the next stage if they meet the speciﬁed condition)


$sort     (Sorts the field we created during the group stage)


$set      (Update only applied to first matching document)


$inc      (Increments field by specified value)


$unset    (Used to remove speciﬁed ﬁelds)


$rename   (Renames specified field)


$pop      (Removes either the ﬁrst or last value of an array {-1} first element, {1} last element)


$push     (Adds a value to the end of an array)


$addToSet (Adds a value to the end of an array unless it is already present)


$pull     (Remove any instance of a value from an array)


$group    (Used to group data by any field we specify)


$project  (Limits the ﬁelds we send)


$limit    (Specify the number of documents to limit)



# Data types

Documents are persisted in a format called BSON

Strings   " "


Numbers   546


Booleans  true


Arrays    ["caracteristic", "caracteristic"]


Objects   {"Attribute" : "caracteristic"}


Null      null


OnjectID  OnjectId(...)


Date      Isodate(...)


# Most commun questions

#Explain what is MongoDB?

Mongo-DB is a document database which provides high performance, high availability and easy scalability.


#What is “Namespace” in MongoDB?

MongoDB stores BSON (Binary Interchange and Structure Object Notation) objects in the collection. The concatenation of the collection name and database name is called a namespace.


#What is sharding in MongoDB?

The procedure of storing data records across multiple machines is referred as Sharding. It is a MongoDB approach to meet the demands of data growth. It is the horizontal partition of data in a database or search engine. Each partition is referred as shard or database shard.


#How can you see the connection used by Mongos?

To see the connection used by Mongos use db_adminCommand (“connPoolStats”);


#Explain what is a replica set?

A replica set is a group of mongo instances that host the same data set. In replica set, one node is primary, and another is secondary. From primary to the secondary node all data replicates.


#How replication works in MongoDB?

Across multiple servers, the process of synchronizing data is known as replication. It provides redundancy and increase data availability with multiple copies of data on different database server. Replication helps in protecting the database from the loss of a single server.


#Mention what is the command syntax for inserting a document?

For inserting a document command syntax is database.collection.insert (document).


#Mention how you can inspect the source code of a function?

To inspect a source code of a function, without any parentheses, the function must be invoked.


#What is the command syntax that tells you whether you are on the master server or not? And how many master does MongoDB allow?

Command syntax Db.isMaster() will tell you whether you are on the master server or not. MongoDB allows only one master server, while couchDB allows multiple masters.


#Mention the command syntax that is used to view Mongo is using the link?

The command syntax that is used to view mongo is using the link is db._adminCommand(“connPoolStats.”)


#Explain what are indexes in MongoDB?

Indexes are special structures in MongoDB, which stores a small portion of the data set in an easy to traverse form. Ordered by the value of the field specified in the index, the index stores the value of a specific field or set of fields.


#Mention what is the basic syntax to use index in MongoDB?

The basic syntax to use in MongoDB is >db.COLLECTION_NAME.ensureIndex ( {KEY:1} ). In here the key is the the name of the COLUMN (or KEY:VALUE pair) which is present in the documents.


#Explain what is GridFS in MongoDB?

For storing and retrieving large files such as images, video files and audio files GridFS is used. By default, it uses two files fs.files and fs.chunks to store the file’s metadata and the chunks.
