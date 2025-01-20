FROM apache/spark:3.5.4-scala2.12-java17-python3-r-ubuntu
USER root
RUN mkdir /home/spark && chown spark:spark /home/spark
USER spark
ENV PYTHONPATH="${PYTHONPATH}:${SPARK_HOME}/python:${SPARK_HOME}/python/lib/py4j-0.10.9.7-src.zip:/home/spark/.local/bin"
ENV PATH="${PATH}:/opt/spark/python/bin:/opt/spark/bin"