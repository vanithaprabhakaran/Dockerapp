
# start by pulling the python image
FROM python:3.8

# install dependencies
#RUN pip3 install --upgrade pip
#RUN pip3 install psutil
#RUN pip3 install flask
#RUN pip3 install flask_cors
#RUN pip3 install streamlit

#RUN pip install -r requirements.txt


# copy the requirements file into the image
COPY ./requirements.txt /app/requirements.txt

# switch working directory
WORKDIR /app

# install the dependencies and packages in the requirements file
RUN pip3 install -r requirements.txt

# copy every content from the local file to the image
COPY . /app


ENTRYPOINT [ "python3" ]

CMD ["app.py" ]
