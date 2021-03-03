# Anton Gorbachev

### Contacts:
* [GitHub](https://github.com/1Gluk1) : 1Gluk1
* [VKontakte](https://vk.com/evol_way) : evol_way
* Email : gorbachovanton@yandex.ru
* Phone : +7-(996)-938-23-89
* _Location :_ _Russia, Tomsk_

#### Desired position
* Junior full-stack (MERN) devoloper

### About me
I am 23 years old, won school programming olympiads on Pascal. Now I am studying Full-Stack development with great interest, I want to learn how to make useful web applications for people.

### Skills:
* HTML/HTML5, CSS/CSS3
* Core JavaScript / ES6
* BEM, Sass. WebPack
* React, Redux, Express, MongoDB, Node.js
* Agile, Scrum
* Figma, Adobe Photoshop

### My code:
```python
# coding: utf-8

from horoscope import generate_prophecies
from datetime import datetime as dt

def generate_page(head, body):
    page = f"<html>{head}{body}</html>"
    return page

def generate_head(title):
    head = f'''<meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="ie=edge">
    <title>{title}</title>'''
    return f'<head>{head}</head>'

def generate_body(header, paragraphs):
    body = f"<h1>{header}</h1>"
    for p in paragraphs:
        body = body + f"<p>{p}</p>"
    return f"<body>{body}<hr><a href='about.html'>О реализации</a></body>"

def save_index_page(title, header, paragraphs, output="index.html"):
    fp = open(output, "w", encoding="utf8")
    today = dt.now().date()
    page = generate_page(head=generate_head(title), body=generate_body(header=header, paragraphs=paragraphs))
    print(page, file=fp)
    fp.close()
    
today = dt.now().date()
save_index_page(title="Гороскоп на сегодня", header="Ваши предсказания на " + str(today), paragraphs=generate_prophecies())
```

### Education:
* TSU Faculty of Physics and Technology, Department of Mahatronics and Robotics - 3 course.

### Courses:
* EPAM - Computer Science Basic
* Odin project - Full-stack JS devoloper
* Way of the Samurai - React/Redux

### Languages:
* English (B1)