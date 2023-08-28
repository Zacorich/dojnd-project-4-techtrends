# use python 3.8
FROM python:3.8-slim

# set working directory
WORKDIR /app

# copy file with defined dependencies to working directory
COPY ./techtrends/requirements.txt .

# install python dependencies using the file
RUN pip install --no-cache-dir -r requirements.txt

# copy project contents to the working directory
COPY ./techtrends/ .

# define command to run when container starts
CMD sh -c "python init_db.py && python app.py"

# open networking port 3111
EXPOSE 3111
