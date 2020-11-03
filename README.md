# simple-streaming
Simple RTMP streamin service

# Quick Start
    mkdir -p mp4s
    wget http://<video-url> -o mp4s/sample.mp4
    https://github.com/dukov/simple-streaming
    cd simple-streaming
    kind create cluster --config kind-cluster.yaml
    kustomize build config/video-on-demand | kubectl apply -f -
    kustomize build config/transcoder | kubectl apply -f -
    vlc rtmp://localhost/pull
