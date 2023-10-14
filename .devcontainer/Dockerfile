# 使用來自 Docker Hub 上的 Node.js 映像
FROM node:18

# 設定工作目錄
WORKDIR /app

# 複製 package.json 和 package-lock.json 到容器中
COPY package.json package-lock.json ./

# 安裝必要的依賴（使用 npm ci）
RUN npm ci

# 複製整個目錄的文件到容器中（可以包括應用程式代碼等）
COPY . .