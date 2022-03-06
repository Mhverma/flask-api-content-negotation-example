Installation Requirments

* python 3.9
* flask

Virtual envionement

1. First unzip  the project and move to project directory
2. Then you can create a new virtual environment with the command:

   ```
   $ python3 -m venv venv
   ```
3. Activate the virual environment:

   ```
   source venv/bin/activate
   ```
4. Install Flask

```
pip install flask
```

Start Application

1. Run below command to start the application

   ```
   python3 app.py
   ```
3. Curl command without header

   ```
    curl  http://localhost:8000/hello
   ```

   output:

   ```
   <p>Hello, World</p>
   ```
4. Curl command with header:

   ```
   curl -H "accept:application/json" http://localhost:8000/hello
   ```

output:

```
{
  "message": "Hello, Wrold"
}
```

Enable Debug option

* start application with debug option

```
python3 app.py debug
```

* Logging sample:

2022-03-06 12:21:32,614 DEBUG app Thread-3 : [2022-Mar-06 12:21] /hello?
