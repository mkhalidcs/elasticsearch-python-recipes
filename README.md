# elasticsearch-python-recipes

## 1. Install Docker:
  Follow the official Docker installation guide based on your operating system:<br />
  * [Docker Installation Guide](https://docs.docker.com/engine/install/)

## 2. Start Elasticsearch with Docker:
  Run the following commands in your terminal to start a single-node Elasticsearch cluster:
  ```
  docker pull docker.elastic.co/elasticsearch/elasticsearch:7.16.3
  docker run -d -p 9200:9200 -e "discovery.type=single-node" docker.elastic.co/elasticsearch/elasticsearch:7.16.3
  ```

  Ensure that Elasticsearch is up and running by visiting [http://localhost:9200](http://localhost:9200) in your web browser.
  Additional Docker commands for managing Elasticsearch containers can be found in the [official Elasticsearch Docker documentation](https://www.elastic.co/guide/en/elasticsearch/reference/current/docker.html).

## 3. Install Jupyter Notebook:
Open your command line and install Jupyter Notebook using:

```
pip install jupyter
```

## 4. Create a Virtual Environment:
  It's a good practice to use virtual environments to manage packages. Create a virtual environment using:
  ```
  python -m venv myenv
  source myenv/bin/activate  # On Windows, use 'myenv\Scripts\activate'
  ```

## 5. Install Required Packages:
  Inside your virtual environment, install the necessary Python packages:
  ```
  pip install pandas elasticsearch
  ```

## 6. Launch Jupyter Notebook:
  Start Jupyter Notebook by running the following command in your terminal:

  ```
  jupyter notebook
  ```

  
