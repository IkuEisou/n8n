# 使用 n8n 官方运行器镜像作为基础
FROM n8nio/runners:latest

# 切换到 root 用户来安装软件
USER root

# 使用 uv 安装 pandas 等库到 n8n Python 运行器的虚拟环境
RUN uv pip install --python /opt/runners/task-runner-python/.venv/bin/python \
    pandas \
    openpyxl \
    requests \
    numpy

# 切回默认用户
USER runner