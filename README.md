
## 安装
### 1、Docker
```
docker pull realwang/nas-tools-unlock
```
教程见 [这里](docker/readme.md) 。

如无法连接Github，注意不要开启自动更新开关(NASTOOL_AUTO_UPDATE=false)，将NASTOOL_CN_UPDATE设置为true可使用国内源加速安装依赖。

### 2、本地运行
python3.10版本，需要预安装cython，如发现缺少依赖包需额外安装：
```
git clone -b master https://github.com/Hiddenl/nas-tools-unlock --recurse-submodule 
python3 -m pip install -r requirements.txt
export NASTOOL_CONFIG="/xxx/config/config.yaml"
nohup python3 run.py & 
```

### 3、可执行文件
下载打包好的执行文件运行即可，会自动生成配置文件目录：

https://github.com/Hiddenl/nas-tools-unlock/releases
