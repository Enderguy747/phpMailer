# phpMailer
simple php mailer class



## Installation
just copy the the mail folder in your proyect and change the class as much as you need! :)


## Change the atributes for yours in the SendEmail class constructor
```php
 function __construct()
    {
        $this->mail       = new  PHPMailer(true);
        $this->host       ="smtp.gmail.com"; // if you are using gmail
        $this->SMTPAuth   =true;
        $this->Username   ="your email address";
        $this->Password   ="your password"; //you need to generate a password for applications in gmail 
        $this->SMTPSecure ="TLS";
        $this->Port       =587;
        
        $this->mailFrom   ="your mail *again";
        $this->mailSender ="your email title";
    }

```



## How to use the class

```php
               //crate a sendEmail object
                $sm = new SendEmail();
                //use the newEmail method and give it the necesary params 
                $mail = $sm->newEmail("", "", $destinationMail, "Verificacion ", "Su codigo es", "param", "");

                if ($mail === true) {

                    //do something
                    echo "sended";
                } else {
                    //do something
                    echo "error";
                }
```
## Do not forget import the classes
```php
include '../mail/SendEmail.php';
```
  

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## Lets get in touch
[Text me](https://www.facebook.com/jose.rodriguessotela)

 
