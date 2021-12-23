FROM nginx:stable
RUN rm /etc/nginx/conf.d/*
COPY hello.conf /etc/nginx/conf.d/
COPY index.html /usr/share/nginx/html/
COPY style.css /usr/share/nginx/html/
COPY udacity-logo.png /usr/share/nginx/html/
RUN pip install --upgrade pip &&\
    pip install --trusted-host pypi.python.org -r requirements.txt
