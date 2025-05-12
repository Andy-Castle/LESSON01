# Esta es la lección 1

py -m venv .venv

.venv\Scripts\activate

py -m pip install Django

django-admin startproject myproject

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01> cd .\myproject\

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01\myproject> py manage.py runserver

## Esta es la lección 2

Esto es la sección 2 de la lección

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01\myproject>
py manage.py startapp posts

### Esta es la lección 3

Esto es la sección3 de la lección

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01\myproject> py manage.py migrate

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01\myproject> py manage.py makemigrations

#### Esta es la lección 4

Esto es la sección 4 de la leccion

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01\myproject> py manage.py shell

Python 3.13.3 (tags/v3.13.3:6280bb5, Apr 8 2025, 14:47:33) [MSC v.1943 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)

> > > from posts.models import Post
> > > p = Post()
> > > p
> > > <Post: Post object (None)>
> > > p.title = "Mi primer Post!"
> > > p.save()
> > > Post.objects.all()
> > > <QuerySet [<Post: Post object (1)>]>
> > > exit()

(.venv) PS C:\Users\maste\Desktop\Python\DjangoCourse\LESSON01\myproject> py manage.py shell
7 objects imported automatically (use -v 2 for details).

Python 3.13.3 (tags/v3.13.3:6280bb5, Apr 8 2025, 14:47:33) [MSC v.1943 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
(InteractiveConsole)

> > > from posts.models import Post
> > > p = Post()
> > > p.title = "Mi segundo Post"
> > > p.save()
> > > Post.objects.all()
> > > <QuerySet [<Post: Mi primer Post!>, <Post: Mi segundo Post>]>
> > > exit()
> > > now exiting InteractiveConsole...
