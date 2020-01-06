```
python3 -m venv env
source env/bin/activate
pip install -r requirements.txt
```

```
cython hello.py --embed
```

```
gcc -Os -I /usr/include/python3.6m -o hello hello.c -lpython3.6m -lpthread -lm -lutil -ldl
```
