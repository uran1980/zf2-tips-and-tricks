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
