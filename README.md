# phpMailer
simple php mailer class



## Installation
just copy the the mail folder in your proyect and change the class as much as you need! :)



## How to use the class

```php
 $sm = new SendEmail();
                $mail = $sm->newEmail("", "", $vector[0]['correo'], "Verificacion ", "Su codigo es", $_SESSION["codigo"], "");




                if ($mail === true) {

                    header("Location: /ProyectoWebII/components/userView/2stepCode.php");
                    echo "sended";
                } else {
                    echo "error";
                }
```
  

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Lets get in touch
[Text me](https://www.facebook.com/jose.rodriguessotela)

 
