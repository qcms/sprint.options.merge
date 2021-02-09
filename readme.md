## example how to use multiple merged files in sprint.options.php

sprint.options.php not ready for big projects with many tabs and really big array

example  `sprint.options.php`

```php
<?
return array_merge(
    include (__DIR__.'/sprint.options.PART_ONE.php'),
    include (__DIR__.'/sprint.options.PART_TWO.php')
);
```

example `sprint.options.PART_ONE.php`

```php
<?
return [
	'PART_ONE_TEST1' => array(
		'TITLE' => 'TEST 1 name',
		'DEFAULT' => '',
		'WIDTH' => '800',
		'HEIGHT' => '100',
		'TAB' => 'TEST 1 tab',
	),
	'PART_ONE_TEST2' => array(
		'TITLE' => 'TEST 2 name',
		'DEFAULT' => '',
		'WIDTH' => '800',
		'HEIGHT' => '100',
		'TAB' => 'TEST 1 tab',
	),
	'PART_ONE_TEST3' => array(
		'TITLE' => 'TEST 3 name',
		'DEFAULT' => '',
		'WIDTH' => '800',
		'HEIGHT' => '100',
		'TAB' => 'TEST 1 tab',
	),
];
```

example `sprint.options.PART_TWO.php`

```php
<?
return [
	'PART_TWO_TEST1' => array(
		'TITLE' => 'TEST2 1 name',
		'DEFAULT' => '',
		'WIDTH' => '800',
		'HEIGHT' => '100',
		'TAB' => 'Second tab',
	),
	'PART_TWO_TEST2' => array(
		'TITLE' => 'TEST2 2 name',
		'DEFAULT' => '',
		'WIDTH' => '800',
		'HEIGHT' => '100',
		'TAB' => 'Second tab',
	),
	'PART_TWO_TEST3' => array(
		'TITLE' => 'TEST2 3 name',
		'DEFAULT' => '',
		'WIDTH' => '800',
		'HEIGHT' => '100',
		'TAB' => 'Second tab',
	),
];
```