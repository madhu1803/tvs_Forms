# TVS-FORMS

## Project Structure - tvs_forms

```
tvs_forms/ => project root
   app.py => contains config for this app
   forms.py => contains fields mapped to the forms
   templates/ => contains all the templates (html files & UI)
      includes/ => sections used often
         dummy_sidebar.html => side bar
         footer.html => footer
         sidebar.html => sidebar
         topnav.html => navigation bar
      main_tables/ => contains 3 forms
         table1.html => form1
         table2.html => form2
         table3.html => form3
   static/ => project level static files
      audio
      css
      img
      scripts
      vendor
```

## Project Structure - Mysql Database

```
madhu_db1/ => database => 3 tables
   form1 => 2 initial fields(id,date)
   form2 => 2 initial fields(id,date)
   form3 => 2 initial fields(id,date)
```

## Getting Started | development (Mysql database)

1. Run the Apache server & mysql database in Xampp
2. visit Localhost => PhpmyAdmin
3. create database
4. create 3 tables => form1,form2,form3 with fields id & date

## Getting Started | development

1. Create a virtualenv `python3 -m venv venv`
2. Activate the virtualenv `. venv/bin/activate`
3. upgrade pip `pip install --upgrade pip`
4. Install requirements `pip install -r requirements.txt`
5. Run the dev server `python app.py`

## Getting Started | Routes

1. `/` or `/create` - insert new data or update existing data into db or view today's data
2. `/detail` - view data by date
