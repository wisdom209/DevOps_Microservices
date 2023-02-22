FROM python:3.7.3-stretch

# working directory
WORKDIR /app

# copy source code to working dir
COPY . flask_app/web.py /app/
COPY . nlib /app/

# install packages
RUN pip install --upgrade pip &&\
	pip install -r requirements.txt

# Expose port 80
EXPOSE 80

# run app.py on container launch
CMD ["python", "web.py"]
