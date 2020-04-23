# PhpStorm WP Live Templates
Мой набор шаблонов(шорткодов) для разработки на WP.

## Установка

Для установки шаблоновЮ скопируйте все файлы из репозитория в папку `templates` по адресу [Config Directory](https://www.jetbrains.com/help/phpstorm/tuning-the-ide.html#config-directory)

Обычное расположение папки конфигурации

### Windows:
```
Syntax
%HOMEPATH%\.<product><version>\config
Example
C:\Users\JohnS\.PhpStorm2020.1\config
```

### macOS:
```
Syntax
~/Library/Preferences/<product><version>
Example
~/Library/Preferences/PhpStorm2020.1
```

### Linux:
```
Syntax
~/.<product><version>/config
Example
~/.PhpStorm2020.1/config
```

После копирования перезагрузите PhpStorm.


## Дефолтные шорткоды

* Вставить Live Template - <code>CTRL+J</code>
* Окружить with Live Template - <code>CTRL+ALT+J</code>



## WP Templates
1. __ - Transalation
```php
__( $SELECTION$, '$textdomain$' );
```

2. **aa** - Add action hook
```php
add_action( '$hook$', '$callback$' );
```

3. **aafu** - Add action with function
```php
add_action( '$hook$', function () {
	//your code
} );
```

4. **aam** - Add Action with method
```php
add_action( '$hook$', array( $class$, '$method$' ) );
```

5. **af** - Add Filter
```php
add_filter( '$hook$', '$callback$' );
```

6. **afm** - Add Filter with method
```php
add_filter( '$hook$', array( $class$, '$method$' ) );
```

7. **ea** - Escapte Attribute
```php
esc_attr( $SELECTION$ );
```

8. **ip** - Insert Post
```php
// Create post object
$my_post = array(
  'post_title'    => '',
  'post_content'  => '',
  'post_status'   => 'publish',
);

// Insert the post into the database
wp_insert_post( $my_post );
```

9. **rpt** - Register Post Type: Shows same as in sublime text. Since its huge so below is just a sample. When you use it. It will be in full just like in sublime.
```php
function prefix_register_name() {
	$labels = array();
}
```

10. **rt** - Register Taxonomy: Shows same as in sublime text. Since its huge so below is just a sample. When you use it. It will be in full just like in sublime.
```php
function my_taxonomies_name() {

	$labels = array(
		'name'                  => _x( 'Plural Name', 'Taxonomy plural name', 'text-domain' ),
		'singular_name'         => _x( 'Singular Name', 'Taxonomy singular name', 'text-domain' ),
		'search_items'          => __( 'Search Plural Name', 'text-domain' ),
		'popular_items'         => __( 'Popular Plural Name', 'text-domain' ),
		'all_items'             => __( 'All Plural Name', 'text-domain' ),
		'parent_item'           => __( 'Parent Singular Name', 'text-domain' ),
		'parent_item_colon'     => __( 'Parent Singular Name', 'text-domain' ),
		'edit_item'             => __( 'Edit Singular Name', 'text-domain' ),
	);
}
```

11. **wpa** - wp_parse_args
```php
$$$args$ = wp_parse_args( $$$source$, array(
	$key$ => $value$,
) );
```



## jQuery Templates

**cl** - console.log()

