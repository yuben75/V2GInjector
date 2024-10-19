# 使用官方 Python 镜像
FROM python:3.9-slim

# 设置工作目录
WORKDIR /app

# 更新包管理器并安装必要的软件包
RUN apt-get update && apt-get install -y \
    build-essential \
    git \
    curl

# 复制并安装 Python 依赖
COPY requirements.txt /app/
RUN pip install --no-cache-dir -r requirements.txt

# 暴露必要的端口
EXPOSE 8000

# 默认启动命令
CMD ["bash"]