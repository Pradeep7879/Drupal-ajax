# Drupal-ajax
Useful services of ajax in Drupal
---------------------------------


    use Drupal\Core\Ajax\HtmlCommand;
    use Drupal\Core\Ajax\AjaxResponse;
    use Drupal\Core\Ajax\InvokeCommand;
    use Drupal\Core\Ajax\OpenModalDialogCommand;
    

Way to Use in code of HtmlCommand and InvokeCommand 

     $response->addCommand(new HtmlCommand('#intro-text', $this->t('Update Text Here.')));
     
     $response->addCommand(new InvokeCommand('#intro-text', 'css', ["color", "red"]));
     
      return $response;
      
 pop-up open
 
      $response->addCommand(new OpenModalDialogCommand('', $modal_form, ['width' => '400']));
      return $response;
      
      
          
          
