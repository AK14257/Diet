# Use a specific version of Python as the base image
FROM python:3.12.0

# Create the app directory structure
RUN mkdir -p /app/frontend

# Copy the frontend code into the container
COPY Streamlit_Frontend /app/frontend

# Set the working directory inside the container
WORKDIR /app/frontend

# Upgrade pip and install dependencies
RUN pip install --upgrade pip
RUN pip install -r requirements.txt

# Expose the port Streamlit uses
EXPOSE 8501

# Run the Streamlit app
CMD ["streamlit", "run", "Hello.py"]
