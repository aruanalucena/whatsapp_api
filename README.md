![imagem](https://i.imgur.com/mbdq8P5.png)

Cientista de dados em formação , buscando dados, limpando, manipulando, analisando os dados. Criando modelos de Machine Learning supervisionado e não supervisionado. Com dados estruturado e não estruturados. Deploy e storytelling dos projetos . Estudando sempre em evolução.


Conheça mais sobre os meus projetos, publicações na área de dados.
* Meu perfil no [Linkedin](https://www.linkedin.com/in/aruanacortezdatascientist/
* Meu perfil no [Instagram](https://www.instagram.com/aruanacortez_dev/)
* Minha página no [Facebook](https://www.facebook.com/aruanacortez.lucena/)
* Visite meu site [Site](https://www.aruanacortezdev.com.br)
* Conheça minhas publicações [Medium](https://aruanacortezdev.medium.com/)
* Meu canal no [YouTube](https://www.youtube.com/channel/UCdpeqZIZ1JGZk2PywYTcQdw)







# WHATSAPP BOOT DO CURSO AWARI DE DATA SCIENCE


# WhatsApp Group API on Selenium
Easy to use API on selenium to have control of a WhatsApp group using the web browser. 

### Implemented features
- Get all contacts from a selected group
```
In [1]: from whatsapp_api import WhatsApp
In [2]: wp = WhatsApp()
Loading...
Please scan the QR Code and enter in the group
In [3]: wp.get_group_numbers()
```
- Write and/or send messages
```
In [1]: from whatsapp_api import WhatsApp
In [2]: wp = WhatsApp()
Loading...
Please scan the QR Code and enter in the group
In [3]: wp.send_message('This message is going to be sent')
In [4]: wp.write_message('This message is going to be written but not sent')
```
- Search for a contact given a keyword (phone number or name)
```
In [1]: from whatsapp_api import WhatsApp
In [2]: wp = WhatsApp()
Loading...
Please scan the QR Code and enter in the group
In [3]: wp.search_contact('+55000000000')
```
- Phone number parser to the same standard for performing set operations:
```
    >>> group_numbers = wp.get_group_numbers()
    >>> group_numbers = wp.parser(group_numbers[:-1]) # Remove last contact which is not a number ('You')
    >>> all_numbers = [...]
    >>> # Numbers should start with the country code, for example +55
    >>> all_numbers = wp.parser(all_numbers)
    >>> not_joined = all_numbers - group_numbers
```

- Get last message
```
    >>> wp.get_last_message()
```

- Get all messages
```
    >>> wp.get_all_messages()
```

### Tutorial on Udemy (in Portuguese)
- https://www.udemy.com/course/aprenda-a-programar-um-bot-do-whatsapp/?couponCode=PRECOMINIMO

### Possible future features
- ?

### Requirements
- Selenium: `pip install selenium`
- ChromeDriver: http://chromedriver.chromium.org/
    - After downloading chromedriver, make sure to add in a folder accessible from the PATH

### LICENSE
MIT
