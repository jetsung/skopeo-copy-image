# 复制镜像

## 环境变量
将值复制粘贴至后台配置，变量名为 `DOCKER_CONFIG_JSON`。
```bash
# cat ~/.docker/config.json |xsel -b
DOCKER_CONFIG_JSON=$(cat ~/.docker/config.json |xsel -b)
export DOCKER_CONFIG_JSON
```
