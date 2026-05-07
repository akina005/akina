curl -L -o /tmp/ffmpeg.tar.xz https://github.com/akina005/akina/releases/download/ffmpeg/ffmpeg-release-amd64-static.tar.xz
mkdir -p /tmp/ffmpeg-static
tar -xf /tmp/ffmpeg.tar.xz -C /tmp/ffmpeg-static --strip-components=1
sudo ln -sf /tmp/ffmpeg-static/ffmpeg /usr/local/bin/ffmpeg
sudo ln -sf /tmp/ffmpeg-static/ffprobe /usr/local/bin/ffprobe
ffmpeg -version
