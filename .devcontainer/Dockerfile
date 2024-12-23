# ROS Noeticのベースイメージを使用
FROM osrf/ros:noetic-desktop-full

# 基本的なツールをインストール
RUN apt-get update && apt-get install -y \
    python3-colcon-common-extensions \
    python3-pip \
    build-essential \
    git \
    vim \
    && rm -rf /var/lib/apt/lists/*

# ワークスペースを作成
RUN mkdir -p /workspace/src
WORKDIR /workspace

# ROS環境の設定をソースする
RUN echo "source /opt/ros/noetic/setup.bash" >> /root/.bashrc
