FROM node:18

WORKDIR /app

# Copy package.json và package-lock.json
COPY package*.json ./

# Sao chép toàn bộ mã nguồn và các file khác vào container
COPY ./ ./

# Tạo thư mục certs nếu chưa có
RUN mkdir -p /app/certs

# Sao chép các file chứng chỉ vào thư mục /app/certs trong container
COPY ./privkey.pem /app/certs/privkey.pem
COPY ./fullchain.pem /app/certs/fullchain.pem
COPY ./chain.pem /app/certs/chain.pem

# Cài đặt các package cần thiết
RUN npm install nodemon
RUN npm install

# Lệnh mặc định để chạy ứng dụng
CMD ["npm", "start"]
