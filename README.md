# nginx 分享配置 模块化

## 1. http

```sh

# http块
http
{
    # http全局块

     # 在此处加载 nginx conf
    include {absolute path}/*.conf;
    ...
    # 虚拟主机server块
    server {
        # server全局块
        ...
        # location块
        location [PATTERN]
        {
            ...
        }
        location [PATTERN]
        {
            ...
        }
    }
    server
    {
      ...
    }
    # http全局块
    ...
}

```
