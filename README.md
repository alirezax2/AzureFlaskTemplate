# AzureFlaskTemplate
a template for python Flask Web App with Azure Identity


Login in Azure Portal, search for App Registration and create a new app registration; select single tenant. 
Follow web application in Quickstart, select python and click to complete step 1 and copy generate secret key as SECRET_ID. Copy TENANT_ID (Directory (tenant) ID) and CLIENT_ID (Application (client) ID)

Step 1: Configure your application in Azure portal
For the code sample in this quickstart to work:

Add a reply URL as http://localhost:5000/getAToken.
Create a Client Secret.
Add Microsoft Graph API's User.ReadBasic.All delegated permission.

in microsoft github repo, version of flask session needed to be update (requirements.txt) 
for local run, needed to load_dotenv() in app_config.py

replace TENANT_ID, SECRET_ID and CLIENT_ID in .env file

make virtual env, activate, install libs with pip and run web app

```
python -m venv myenv
```

```
.\myenv\Scripts\activate.bat
```

```
 ./myenv/bin/activate
```

```
pip install -r requirements.txt
```

```
flask run --debug --host=localhost --port=5000
```