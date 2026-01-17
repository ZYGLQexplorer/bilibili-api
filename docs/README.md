![Bilibili API Logo](logo.png)

<div align="center">

**欢迎来到 bilibili-api 文档 ヾ(ﾟ∀ﾟゞ)**

</div>

bilibili-api 是一个调用 [Bilibili](https://www.bilibili.com) API 的 Python 库，除此之外还有其他相关功能提供。

模块可调用的 API 范围包括视频、音频、专栏（图文）、番剧、动态、用户、直播、个人消息中心，等等。模块内置了这些功能相关接口的信息，提供了方便的函数调用，省去了找接口、验参数与部分接口应用风控参数的常规接口接入过程。

## 安装

``` zsh
# 正式版本
$ pip3 install bilibili-api-python

# dev 分支版本，最新修改都在此处。
$ pip3 install git+https://github.com/Nemo2011/bilibili-api.git@dev

# dev-dyn-fp 分支版本
$ pip3 install git+https://github.com/Nemo2011/bilibili-api.git@dev-dyn-fp

# 开发版本
$ pip3 install bilibili-api-dev
```

除此之外，模块还需要 **至少一个** 异步网络请求库，默认支持 `curl_cffi` `aiohttp`
`httpx`。

``` zsh
# aiohttp
$ pip3 install aiohttp
$ pip3 install "aiohttp[speedups]" # faster

# httpx
$ pip3 install httpx
$ pip3 install "httpx[http2]" # http2 support

# curl_cffi
$ pip3 install "curl_cffi"
```

## 指纹伪装

模块支持 [`curl_cffi`](https://github.com/lexiforest/curl_cffi) + [`fpgen`](https://github.com/scrapfly/fingerprint-generator) 指纹伪装。当然，两个模块都需要单独安装。

``` zsh
$ pip3 install "curl_cffi"
$ pip3 install fpgen

# 不过也可以
$ pip3 install "bilibili-api-python[fingerprint]"
```

## 快速上手

## 配置项

## 常见问题
