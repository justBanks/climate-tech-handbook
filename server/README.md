#### Setting Up Flask App

###### 1. Change working directory to this directory

```
cd server
```

###### 2. Create a virtual environment

Python 3.4 or above:

```
python -m venv venv
```

otherwise you can use:

```
pip install virtualenv
virtualenv venv
```

###### 3. Activate virtual environment

Linux or MacOS:

```
source venv/bin/activate
```

Windows (cmd.exe):

```
venv\Scripts\activate.bat
```

Windows (Powershell):

```
venv\Scripts\Activate.ps1
```

###### 4. Install the required packages. 

```
pip install -r requirements.txt
```

#### Running the Flask App

If you completed the installation process without any persisting errors, you can continue. If you need further assistance, open an [issue](https://github.com/climate-tech-handbook/data-magic/issues/new).

###### 1. Run the Flask app with `flask run` or try `python app.py`
###### 2. The app will create a file for a specific topic using the prompts, templates, and configurations provided in the `data` folder.
   - At this moment in the app it's being forced with a `@before_request` decorator, this will be improved upon in the future.
###### 3. The generated file will be saved in the `output_test` folder.