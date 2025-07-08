FROM ubuntu@sha256:440dcf6a5640b2ae5c77724e68787a906afb8ddee98bf86db94eea8528c2c076

RUN apt-get update && apt-get install -y wget && rm -rf /var/lib/apt/lists/*

RUN wget -O /bazel-remote https://github.com/withered-magic/bazel-remote/releases/download/2025.28.0/bazel-remote-2025.28.0-linux-amd64 && \
    chmod +x /bazel-remote

ENTRYPOINT [ "/bazel-remote" ]
