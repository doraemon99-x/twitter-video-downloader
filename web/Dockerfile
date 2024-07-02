# Gunakan image Node.js sebagai base image
FROM node:16-alpine

# Tentukan direktori kerja di dalam container
WORKDIR /web

# Salin package.json dan package-lock.json ke direktori kerja
COPY package*.json ./

# Install dependencies
RUN npm install

# Salin semua file dan direktori dari project ke direktori kerja
COPY . .

# Tentukan port yang akan digunakan
EXPOSE 3000

# Jalankan aplikasi Next.js
CMD ["npm", "run", "dev"]
