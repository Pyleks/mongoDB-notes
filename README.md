# MongoDB Notes

#### Push To: https://github.com/Pyleks/mongoDB-nKotes.git

#### Basics
Connect to mongoDB with following Command
>  mongo "mongodb+srv://myamazingcluster-96wib.mongodb.net/myTestDB" --username myRoot

##### Basic mongoDB commands
> Show collections - Shows how many DB's there is in the cluster, and which one.  

> coll = db.myFirstMDB - Assign  

> coll.insert({ first: 'john', last: 'lennon', dob: '09/10/1940', gender: 'm', hair_color: 'brown', nationality: 'english', occupation: 'beatle' });

> coll.find() - Can see everything we added  

> coll.find({gender: 'f'});

> coll.find({gender: 'f', nationality: 'english'}); - Find everything with gender f and nationality english  

> coll.find({gender: 'f', $or: [{nationality: 'american'}, {nationality: 'irish'}]});

> coll.find({gender: 'f', $or: [{nationality: 'american'}, {nationality: 'irish'}]});  

> coll.update ({nationality: 'irish'}, {$set: {hair_colour: 'purple'}}, {multi:true});  

> coll.remove({first: 'john', last: 'lennon'});

