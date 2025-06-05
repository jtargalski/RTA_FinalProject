# RTA_FinalProject

# jupyterlab
Python with Spark env for real time data analysis.
```bash
py -m venv venv
venv\Scripts\activate
pip install --no-cache-dir --upgrade pip setuptools
pip install cookiecutter
cookiecutter https://github.com/sebkaz/jupyterlab-project
cd .cookiecutters\jupyterlab-project
docker compose up
```
After composing the Docker containers, go to localhost:8080 to use the JupyterLab.

First, run the terminal in the JupyterLab and install the following missing packages for the project:

```bash
pip install pymongo streamlit altair
```
Then, download the code from this repository - producer.py, consumer.py, app.py.

Run the codes in separate terminals in JupyterLab by using the following commands:

```bash
python producer.py
python consumer.py
streamlit run app.py
```

Then, the live dashboard will be live on localhost:4040

## stop

```bash
ctrl + c 
docker compose down
```
