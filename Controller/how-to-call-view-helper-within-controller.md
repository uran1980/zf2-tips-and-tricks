How to call view helper within Controller
=========================================

v1:
```php
$serverUrl = $this->getServiceLocator()->get('ViewHelperManager')->get('serverUrl')->__invoke(true);
```

v2:
```php
$serverUrlHelper = new Zend\View\Helper\ServerUrl();
$serverUrl = $serverUrlHelper->__invoke(true);
```

@param  string|bool ```$requestUri``` - [optional] if true, the request URI found in **$_SERVER** will be appended as a path.

If a string is given, it will be appended as a path.

Default is to not append any path.
