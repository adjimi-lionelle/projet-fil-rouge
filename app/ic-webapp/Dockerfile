FROM python:3.6-alpine

LABEL maintainer="Adjimi Lionelle"

WORKDIR /opt

COPY . /opt

RUN pip install --no-cache-dir Flask

EXPOSE 8085

ENV ODOO_URL=""
ENV PGADMIN_URL=""

ENTRYPOINT ["/bin/sh", "/opt/init.sh"]
CMD ["python", "app.py"]
