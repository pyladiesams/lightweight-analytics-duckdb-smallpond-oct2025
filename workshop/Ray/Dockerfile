FROM rayproject/ray:latest-py311-cpu

USER root
ENV PATH "/home/ray/anaconda3/bin:$PATH"
ENV PYTHONUNBUFFERED=1
ENV PYTHONDONTWRITEBYTECODE=1

USER ray
WORKDIR /home/ray

COPY requirements.txt .

# Install dependencies
RUN pip install --no-cache-dir --upgrade pip && \
    pip install --no-cache-dir -r requirements.txt

EXPOSE 6379 8265 10001

CMD ["bash"]
