![Project Banner](https://banner.natmfat.com/api/banner?title=Passkey&description=Yet%20another%20password%20manager&stack=python,sqlite,docker)

## Usage

First, activate `pipenv` and create a new "global password" or account.

```bash
python -m pipenv shell
python global_password.py
```

To merge existing passwords from a browser, export the passwords as a CSV file (usually found in settings) and copy the contents into `/passwords/passwords.csv`.

```bash
python password_merge.py
```

Start the Python Bottle server and go to `localhost:5500`

```bash
python main.py
```

## Usage (with Docker)

```
docker build -t password-manager .
docker run -d -p 5500:5500 password-manager
```
