<strong>Developed with python 3.8</strong>
<br /><br />
Install graphene-django<br />
pip install django graphene_django

Migration<br />
python manage.py makemigrations<br />
python manage.py migrate

Example query <br/>
URL: http://127.0.0.1:8000/graphql

<code>
query {
  categoryByName(name:"Meat"){
    id, name,
    ingredients {
      id,
      name
    }
  }
}
</code>