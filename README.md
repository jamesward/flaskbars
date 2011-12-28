Getting Started with Python, Flask, SQLAlchemy, JSON, JQuery, and Heroku
========================================================================

Run Locally
-----------

1. Setup virtualenv

2. Setup PostgreSQL
    
    Set the `DATABASE_URL` environment variable to point to your PostgreSQL server:
    
        export DATABASE_URL=postgres://foo:foo@localhost/helloheroku
    
    Create the database schema:
    
        python manage.py createDbSchema

3. Start Flask Server
    
        python web.py

4. Test out the app

    [http://localhost:5000](http://localhost:5000)
    

Run on Heroku
-------------

1. Create the app

        heroku create -s cedar

2. Add the Heroku Shared Database Add-on

        heroku addons:add shared-database

3. Deploy the app

        git push heroku master

4. Create the database schema

        heroku run "python manage.py createDbSchema"

5. Open the app in your browser

        heroku open

6. Verify that it works

7. Switch the app to `PROD` mode

        heroku config:add PROD=True

