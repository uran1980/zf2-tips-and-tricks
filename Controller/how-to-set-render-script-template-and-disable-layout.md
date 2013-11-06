How to set render script template and disable layout within Controller
======================================================================

```php
<?php
namespace Application\Controller;

use Zend\Mvc\Controller\AbstractActionController;
use Zend\View\Model\ViewModel;

class IndexController extends AbstractActionController
{
    public function indexAction()
    {
        $view = new ViewModel();
        
        // ----------------------- SET RENDER SCRIPT ---------------------------
        $view->setTemplate('application/test/index');
        
        // ------------------------ DISABLE LAYOUT -----------------------------
        $view->setTerminal(true);
        
        return $view;
    }
}



```
