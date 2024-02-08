# quick query to mysql database from array

this library use for make query from array to insert db and update db. 
to use this library you can install with composer like this. 

```bash
composer require gugusd999/db_query_helper
```

below example to use this library.
```php
<?php
require_once "vendor/autoload.php";

use Gugusd999\DbQueryHelper;
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