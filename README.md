setup virtualenv and requirements

```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

create c file

```
cython hello.py --embed
```

build bin file

```
gcc -Os -I /usr/include/python3.6m -o hello hello.c -lpython3.6m -lpthread -lm -lutil -ldl
```

run bin file

```
./hello
```
