# 基于 n8n 官方镜像
FROM n8nio/n8n:2.3.4

# 切换到 root 用户来安装软件
USER root

# 安装 Python3 和 PIP
RUN apk add --update --no-cache python3 py3-pip

# (可选) 如果你需要 pandas, numpy 等库，在这里安装
# RUN pip3 install pandas requests

# 切回 n8n 默认用户 (非常重要，否则启动会报错)
USER node