# Start from a base image
FROM python:3.7-alpine

# Install dependencies
RUN apk add --no-cache --virtual .build-deps gcc musl-dev libffi-dev openssl-dev make \
    && pip install --no-cache-dir notebook \
    && apk del .build-deps

# Set working directory
WORKDIR /notebook

# Expose port for jupyter notebook
EXPOSE 8888

# Run jupyter notebook
CMD ["jupyter", "notebook", "--ip=0.0.0.0", "--port=8888", "--no-browser", "--allow-root"]