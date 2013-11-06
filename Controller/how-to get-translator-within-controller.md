How to get translator within Controller
=======================================

```php
$this->getServiceLocator()->get('translator')->translate($message[, $textDomain][, $locale]);
```

**NOTE:** params in square brackets is optional.
