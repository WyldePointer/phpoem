# phpoem
A PHP tool for displaying Persian poems and also an open database of various poets.

### Usage
```
require "phpoem.php";

$rubais = json_decode(file_get_contents("khayyam.json"));

phpoem_display_rubai($rubais[array_rand($rubais)], "<br />");
```

Result:
```
هر سبزه که بر کنار جویی رُسته‌است
گویی ز لبِ فرشته‌خویی رسته‌است
پا بر سر هر سبزه به خواری ننهی
کان سبزه ز خاک لاله‌رویی رسته‌است

```

### Currently supporting
 - Rubai

<br />
The JSON database files are UTF-8 and their line ending is in Windows format.
<br />
An empty database file(`example_database.json`) is also included so you can populate on your own and contribute if you wish.

<br />
<br />
Special thanks goes to https://ganjoor.net for making these poems available.
