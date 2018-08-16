FROM datastax/dse-server:6.0.2
	
USER root

RUN apt-get update
RUN apt-get -y install python-pip

RUN pip install jupyter
RUN pip install cassandra-driver
RUN pip install tweepy
RUN pip install pattern
RUN pip install pandas

USER dse

VOLUME ["/var/lib/jupyter"]

EXPOSE 8888

ENTRYPOINT [ "/entrypoint.sh", "dse", "exec", "jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--notebook-dir=/var/lib/jupyter"]

