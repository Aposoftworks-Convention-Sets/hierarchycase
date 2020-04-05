# Hierarchy case
This describes a custom case that is a mix between snake case and flat case.

## What it is
Hierarchy case was made for easy reading and understanding of the variable content and reason. It separates the parts of the hierarchy using snake case, and the qualified name of the parts using flat case. The function (reason) of case, if any, should come before the name of it.

### What is considered "hierarchy"?
Hierarchy could be compared to a folder structure, for example, you could have a category, and inside of that, a category only for products (we won't discuss if it's efficient now), that would be the hierarchy, because this product, belongs to the category.

## How to use it
- The function of the case, should come before the name
``` PHP
$id_user = 5;
```
- The hierarchy should be separated by snake case, starting from the top, to the bottom
``` PHP
$id_category_product = 5;
```
- The full name of the hierarchy parts should come with flat case
``` PHP
$email_rafaelcorrea = "rafael.chaves98@hotmail.com";
```
- You can hide the name of variable if only it's function is important or if the name is undefined
``` PHP
$name = "John Doe";
```
- If you are dealing with an array/list/dictionary (or anything of the kind), you pluralize the name in the end of the variable name
``` PHP
$name_users = ["John Doe", "Joe Doe"];
```

## Why use it
- Sometimes you know what the variable is about, but you don't know exactly what is about. For example, if you find a variable declared `$user`, you may not know if it's the actual user object, if it is it's name, or identifier. So giving the type helps you know what exactly you are dealing with. It's placed at the start of the declaration name, so it's easily found, the other important part to be easily found is the actual name, that is in the end of the declaration.
- In most conventions, you may not know if you are dealing with the hierarchy or the full name of the specified variable, as a response, we use two different cases for that. You always know if you are looking at a hierarchy or the full name.
- The actual name of the declared variable, should come last. So you can jump your eyes to the end of the variable, if what you want to know is that.
- If we declared the function as a array, we would miss the actual content of the variable (that could be name, age, id), so instead, we pluralize the name in the end of the variable so you know you are dealing with multiple of whatever is inside of it.

## Examples
``` PHP
$name_active_client = "John Doe";

$name_address_streets = ["Street 1", "Street 2"];

$id_banned_user = "Not you";
```
