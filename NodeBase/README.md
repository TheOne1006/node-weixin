## nodejs 相关支持

1. npm 安装包 `localtunnel`

## 验证公共账号

加密/校验流程如下：
1. 将token、timestamp、nonce三个参数进行字典序排序
2. 将三个参数字符串拼接成一个字符串进行sha1加密
3. 开发者获得加密后的字符串可与signature对比，标识该请求来源于微信
