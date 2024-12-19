# Gunakan base image Python
FROM python:3.9-slim

# Set working directory di container
WORKDIR /app

# Salin file requirements.txt ke dalam container
COPY requirements.txt /app/

# Instal dependencies
RUN pip install --no-cache-dir -r requirements.txt

# Salin semua file aplikasi ke dalam container
COPY . /app

# Expose port 5000 untuk Flask
EXPOSE 5000

# Jalankan aplikasi Flask
CMD ["python", "app.py"]
