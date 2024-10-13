# MongoDb-Operators

## This repository contains the important operators in MongoDb.

### Follow this link to learn more about Query Operators.

https://www.mongodb.com/docs/manual/reference/operator/query/

## Query Operators:-

### 1) `$eq`

#### Matches values that are equal to a specified value. For example:-

```
db.mydb.mycollection.find({"age":{$eq:25}})
```

### 2) `$gt`

#### Matches values that are greater than a specified value. For example:-

```
db.mydb.mycollection.find({"age":{$gt:25}})
```

### 3) `$gte`

#### Matches values that are greater than or equal to a specified value. For example:-

```
db.mydb.mycollection.find({"age":{$gte:25}})
```

### 4) `$in`

#### Matches any of the values specified in an array. For example:-

```
db.mydb.mycollection.find({"age":{$eq:[25, 20]}})
```

### 5) `$lt`

#### Matches values that are less than a specified value. For example:-

```
db.mydb.mycollection.find({"age":{$lt:25}})
```

### 6) `$lte`

#### Matches values that are less than or equal to a specified value. For example:-

```
db.mydb.mycollection.find({"age":{$lte:25}})
```

### 7) `$ne`

#### Matches all values that are not equal to a specified value. For example:-

```
db.mydb.mycollection.find({"age":{$ne:25}})
```

### 8) `$nin`

#### Matches none of the values specified in an array. For example:-

```
db.mydb.mycollection.find({"age":{$nin:[25]}})
```

## Logical Operators:-

### 1) `$and`

#### Joins query clauses with a logical AND returns all documents that match the conditions of both clauses. For example:-

```
db.myCollection.find( { $and: [ { age: { $ne: 30 } }, { city: { $eq: "Los Angles" } } ] } )
```

### 2) `$not`

#### Inverts the effect of a query predicate and returns documents that do not match the query predicate. For example:-

```
db.myCollection.find( { $not: [ { age: { $ne: 30 } }, { city: { $eq: "Los Angles" } } ] } )
```

### 3) `$nor`

#### Joins query clauses with a logical NOR returns all documents that fail to match both clauses. For example:-

```
db.myCollection.find( { $nor: [ { age: { $ne: 30 } }, { city: { $eq: "Los Angles" } } ] } )
```

### 4) `$or`

#### Joins query clauses with a logical OR returns all documents that match the conditions of either clause. For example:-

```
db.myCollection.find( { $or: [ { age: { $ne: 30 } }, { city: { $eq: "Los Angles" } } ] } )
```
