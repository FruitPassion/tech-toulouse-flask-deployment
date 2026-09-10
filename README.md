# Expense Tracker

Expense tracker in Python Flask supports following actions

- Login/Signup
- Add statement
- Delete statement
- Calculate final amount
- Show all statements
- Admin functionality
- Download all statements

## Run the project

> You must have python3 installed on your system before running

> used python 3.10.2 for this project

### Create virtual environment and activate it

```bash
# bash
$ python3 -m venv env

# windows
> python -m venv env
> env\Scripts\activate
```

### Install requirements

```bash
$ pip install -r requirements.txt
```

### Set secret key and database URI

On the Tech Toulouse platform, `DATABASE_URL` (PostgreSQL) and `SECRET_KEY` are
injected automatically as environment variables, nothing to configure.

For local development, set them yourself:

```bash
# bash
(env) $ export DATABASE_URL="postgresql://user:password@localhost:5432/dbname"
(env) $ export SECRET_KEY="secret key"

# windows
(env) > SET DATABASE_URL=postgresql://user:password@localhost:5432/dbname
(env) > SET SECRET_KEY=secret_key
```

Without `DATABASE_URL`, the app falls back to a local `sqlite:///master.sqlite3` file.

### final run
```bash
$ flask run
```