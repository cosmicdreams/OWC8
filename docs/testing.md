#Testing 

## More than just checking things manually
When working on a mid-sized or big project, you can save yourself a lot of frustration if you had tests to give you the 
confidence that all of your features are working properly.  There are many levels of testing (Functional Testing, 
Integration Testing, Unit Testing). Setting up testing for each can be time consuming.  Which is why we wrote this 
guide: to make the process of getting started with testings faster and more cost effective for the client. 

## Functional testing
Tests how functionality works within an application.  You test the end result of the applications actions.  Often times 
what this means is that you're spinning up an actual website and "viewing" the result of the HttpResponse.  Functional 
tests help wrap an application with tests that cover its core functionality.  
  
## Installation 
 
 1. Install Composer:

   ``` 
    php -r "eval('?>'.file_get_contents('https://getcomposer.org/installer'));"
   ```
 
 2. Install the a Behat extension and all of it's dependencies (for your platform) 

    (Drupal)
    
    ```
    php composer.phar require drupal/drupal-extension
    ```
    
    (Wordpress)
        
    ```
    php composer.phar require johnbillion/wordpress-behat-extension
    ```

 3. Copy behat.yml.dist to behat.yml and modify
 
    ```
    cp behat.yml.dist behat.yml
    ```
    
 4. Test to see if Behat can find all of the custom rules

    ```
    bin/behat -dl
    ```

 5. Run Behat and examine test results!
 
    ```
    bin/behat
    ```

### Profiles


Some of the tests need to run on Chrome due to issues in the Selenium Firefox 
driver. To run the tests tagged with @chrome, you need to run Behat using the 
Chrome profile:

    bin/behat --profile chrome

### More information

For detailed instructions, see:

  (Drupal) https://behat-drupal-extension.readthedocs.org/en/3.1/localinstall.html
  (Wordpress) https://github.com/johnbillion/WordPressBehatExtension
