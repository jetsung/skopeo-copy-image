# 复制镜像

## 环境变量
将值复制粘贴至后台配置，变量名为 `DOCKER_CONFIG_BASE64`。
```bash
# 登录数据，并 base64 编码
DOCKER_CONFIG_BASE64=$(cat ~/.docker/config.json | base64 -w 0 | xsel -b)
export DOCKER_CONFIG_BASE64
```
