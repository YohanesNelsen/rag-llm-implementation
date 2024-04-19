# Use a base image that includes Jupyter and PySpark
FROM jupyter/pyspark-notebook:latest

# Install additional Python packages from requirements.txt
COPY requirements.txt /tmp/
RUN pip install --no-cache-dir -r /tmp/requirements.txt

# Perform nltk download
RUN python -m nltk.downloader all

# Copy the entire project directory (including data files) into the Docker image
# Assuming that Dockerfile is in the root of your project directory
COPY . /home/jovyan/work/

# Expose the Jupyter notebook port
EXPOSE 8888

# Start the Jupyter Notebook
CMD ["start-notebook.sh", "--NotebookApp.token=''", "--NotebookApp.password=''"]
