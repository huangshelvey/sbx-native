FROM python:3.10-slim

WORKDIR /app

# 复制当前 python 目录下的依赖文件并安装
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

# 复制所有源码到容器中
COPY . .

# 运行主程序
CMD ["python", "app.py"]
