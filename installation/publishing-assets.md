# Publishing assets

{% hint style="success" %}
Using the Starter Kit? Normally you don't need to worry about publishing assets then. 
{% endhint %}

## Config

```text
php artisan vendor:publish --tag="butik-config"
```

Will be published to `config/butik.php`

{% hint style="info" %}
It's recommended to always publish the config file. 
{% endhint %}

## Views

```text
php artisan vendor:publish --tag="butik-views"
```

{% hint style="success" %}
Use our templates as your starting point
{% endhint %}

Will be published to `resources/views/vendor/butik/`

## Images

```text
php artisan vendor:publish --tag="butik-images"
```

Want to use our SVGs or replace them?

Will be published to `public/vendor/butik/images/`

## Language files

```text
php artisan vendor:publish --tag="butik-lang"
```

If you want to add or edit language files. 

Will be published to `/resources/lang/`

