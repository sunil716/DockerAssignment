FROM httpd:2.4
EXPOSE 80
RUN ServerName=sample-server
RUN echo "\
    <html>\
        <head>\
            <title>Sample Hello World HTML Page</title>\
        </head>\
        <body>\
            <h1>Tag : First<br>This is a sample Hello World HTML Page</h1>\
        </body>\
    </html>" > /usr/local/apache2/htdocs/index.html 