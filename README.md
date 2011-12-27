
1. Setup virtualenv

2. Setup PostgreSQL

export DATABASE_URL=postgres://foo:folocalhost/helloheroku

python
from web import db
db.create_all()

3. Start Flask Server

python web.py




