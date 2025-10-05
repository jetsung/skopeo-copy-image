# 复制镜像

## 环境变量
将值复制粘贴至后台配置，变量名为 `DOCKER_CONFIG_BASE64`。
```bash
# 登录数据，并 base64 编码
DOCKER_CONFIG_BASE64=$(cat ~/.docker/config.json | base64 -w 0 | xsel -b)
export DOCKER_CONFIG_BASE64
```

## 使用方法
1. 复制登录信息的 `base64` 值
```bash
# BASE64 编码后复制
# cat ~/.docker/config.json | base64 -w 0 | xsel -b
cat ~/.docker/config.json | base64 -w 0
```

2. 将值设置至环境变量 `DOCKER_CONFIG_BASE64`

3. 触发复制镜像流水线
```bash
# 源镜像
docker.swagger.io/swaggerapi/swagger-ui:latest

# 目录镜像
sgccr.ccs.tencentyun.com/jetsung/swagger-ui:latest
```
