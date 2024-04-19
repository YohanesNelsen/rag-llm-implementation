# Use a base image that includes Jupyter and PySpark
FROM jupyter/pyspark-notebook:latest

# Install additional Python packages from requirements.txt
COPY requirements.txt /tmp/
RUN pip install --no-cache-dir -r /tmp/requirements.txt

# Copy the entire project directory (including data files) into the Docker image
COPY . /home/jovyan/work/

# Expose the Jupyter notebook port
EXPOSE 8888

# Start the Jupyter Notebook
CMD ["start-notebook.sh", "--NotebookApp.token=''", "--NotebookApp.password=''"]