# quick query to mysql database from array;
this library use for make query from array to insert db and update db. for example you can look code bellow
```php
<?php

$data = [
    [
        "name" => "jhon",
        "gender" => "man",
        "old" => 37
    ]
];

$insertQuery = ArrayToQuery::insert($data, 'my_table', ['id']);
$updateQuery = ArrayToQuery::update($data, 'my_table', 'id');

```