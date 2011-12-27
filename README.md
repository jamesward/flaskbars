Getting Started with Python, Flask, SQLAlchemy, JSON, JQuery, and Heroku
========================================================================

1. Setup virtualenv

2. Setup PostgreSQL
    
    Set the `DATABASE_URL` environment variable to point to your PostgreSQL server:
    
        export DATABASE_URL=postgres://foo:folocalhost/helloheroku
    
    Create the database schema:
    
        python
        from web import db
        db.create_all()

3. Start Flask Server
    
        python web.py
    

