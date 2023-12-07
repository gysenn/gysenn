# configurations such as database connection details

for example, you can use the [db_cred.php](db_cred.php) file like so:
```php
// Include database configuration
include('config/db_cred.php');

// Establish database connection
$conn = new mysqli(DB_HOST, DB_USER, DB_PASSWORD, DB_NAME);

// Check connection
if ($conn->connect_error) {
    die("Connection failed: " . $conn->connect_error);
}
```
