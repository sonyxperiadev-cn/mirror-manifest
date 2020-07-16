# 使用`repo init --mirror`建立`github.com/sonyxperiadev`的本地镜像
```shell
# 初始化
repo init -u https://gitee.com/sonyxperiadev-cn/mirror-manifest --mirror

# 同步仓库
repo sync

# 启动镜像服务
git daemon --verbose --export-all --base-path=. .

```