exo_python
==========

## Requirements

Clone the Vim settings from [here](https://github.com/SenpaiSilver/dotfiles) or set your editor to use tabs instead of spaces.

On Debian 8 as root:
	
	# apt-get install python3 python3-pip
	# pip3 install flask

If `pip3` doesn't work, try `pip`.

## Rules

Unless specified otherwise you must commit **one** file per exercise.

Don't forget to `chmod +x` and use the `#!/usr/bin/env python3` shebang.

Exercises
=========

## 32to64.py

You must print numbers between 32 and 64 included, each number must be printed on the same line.

Example:

	32, 34, 35

Bonus:

* On 64 print a newline instead of a comma.

## MuhJSON.py

You must create the JSON object that will output:

	{
		"key": "value",
		"list": [
				0,
				2,
				4
			]
	}

The order isn't important but the structure must be the same. The file `MuhJSON.py` contains the sample, you must just fill in `data`.

## HelloFlask.py

Create a Flask service that will handle the following requests:

* `GET /` returns `Hello World.`;
* `POST /<path:args>` will print out args but instead of seperating them with slash you will use tabs;
* `GET /date` returns the current date;
* `POST /md5/<str>` returns the MD5 hash of `str`;

Bonus:

* Set the `Content-Type` to plain text so we do not require HTML;

## ls.py

Recode a simple `ls` with no arguments.

Bonus:

* Recode `-l` argument;
* Recode `-R` argument;

## ls-r.py

Recode a recursive `ls` just like if you ran `ls -R`.

## brewing.py

SQL-Alchemy is required, install it with pip:

	# pip3 install sql-alchemy

Create a class mapped to the following table:

* id_user: primary key, auto increment;
* username: string;
* password: string;
* email: string.

Bonus:

* Provide the `.sql` file;
* The class must implement `__repr__`;
* The class can provide à JSON string.
