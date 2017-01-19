# generating-codes
Generate random-looking 5-digit strings consisting of upper and lowercase letters, and numbers. Very lightweight, doesn't repeat for the first 916132832 iterations. You can easily use the same method to get random-looking strings of any length.

Example usage:

```
require("generating_5_digits.php");

$code0 = code_algorithm();
$code1 = code_algorithm();

echo $code0; //"rXzp9"
echo $code1; //"TV8Oi"
```

Crucially, if multiple open process call ```code_algorithm``` at once, there won't be any collisions.

base_helpers.php contains ```convert_to_base_array```, a useful function for representing positive integers with respect to an arbitrary base.
