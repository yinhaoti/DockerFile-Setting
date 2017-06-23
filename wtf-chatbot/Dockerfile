FROM yinhaoti/python-dev-base
MAINTAINER yinhaotian hautienyin@qq.com


# gensim 需要 先安装 numpy 和 scipy，否则会报错
# 先安装 numpy 和 scipy
RUN pip3 install numpy scipy -i https://pypi.tuna.tsinghua.edu.cn/simple
RUN pip3 install -r requirements.txt -i https://pypi.tuna.tsinghua.edu.cn/simple


# 公开80到外部8080端口
# EXPOSE 80:8080

#RUN echo 'python-dev-base创建成功'


# 创建images: docker build -t yinhaoti/python-dev-base .