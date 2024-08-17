## 1. Which base image do you want to use?

FROM python:3.8-slim
## 2. Set the working directory
WORKDIR /app

## 3. Copy the project files into the working directory.
COPY flask-demo/requirements.txt .

## 4. Install the dependencies
RUN pip install -r requirements.txt

EXPOSE 5000

## 5. Document and inform the developer that the application will use PORT 5000 of the container.
COPY flask-demo/ .

ENV FLASK=app.py

## 6. Define the command to run when the container starts.
CMD ["python", "app.py"]