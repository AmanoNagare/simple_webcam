PCに接続されたWebカメラの映像をFlask経由でストリーミング配信し、ローカルネットワーク内の別PCからリアルタイムに映像を受信できるようにするツールです。

Pythonの高速パッケージマネージャーである [uv](https://docs.astral.sh/uv/) を使用することで、環境構築不要ですぐに実行できます。

リポジトリ直下で、 `uv run main.py` を実行してください
起動後
```
* Running on all addresses (0.0.0.0)
* Running on http://127.0.0.1:5000
* Running on http://<あなたのローカルIPアドレス>:5000
```
というメッセージが表示されます。
`http://IPアドレス:5000/video_feed` にカメラが写ります。
cv2.VideoCaptureの引数にそのURLを入れるとそのパソコンのカメラが使えます。