FROM arvindkandhare/filesvc

# Install Python and Basic Python Tools
RUN apt-get install -y python python-dev python-distribute python-pip metapixel
RUN apt-get install -y imagemagick
RUN pip install pika
RUN pip install configparser

ADD . /mosaicme/engine
ADD start_engine.sh /usr/local/bin/

ENTRYPOINT ["bash"]
CMD ["-c","/usr/local/bin/start_engine.sh"]


