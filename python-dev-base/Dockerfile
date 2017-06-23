# 配置基础容器 python-dev-base
FROM python:3.5
MAINTAINER yinhaotian hautienyin@qq.com

# 更新Debian源
RUN mv /etc/apt/sources.list /etc/apt/sources.list.bak && \
echo "deb http://mirrors.163.com/debian/ jessie main non-free contrib" >/etc/apt/sources.list && \
echo "deb http://mirrors.163.com/debian/ jessie-proposed-updates main non-free contrib" >>/etc/apt/sources.list && \
echo "deb-src http://mirrors.163.com/debian/ jessie main non-free contrib" >>/etc/apt/sources.list && \
echo "deb-src http://mirrors.163.com/debian/ jessie-proposed-updates main non-free contrib" >>/etc/apt/sources.list

# 安装自定义package
RUN apt-get update -y && apt-get install -y nano git curl \
    # vim

# 公开80到外部8080端口
# EXPOSE 80:8080

#RUN echo 'python-dev-base创建成功'


# 创建images: docker build -t yinhaoti/python-dev-base .
# 运行到容器: docker run --name pydev -it  yinhaoti/python-dev-base /bin/bash