# 价格保护

如果价格保护运行出错，提示不要频繁点击！

请配置 token

token的获取方式：

1. 运行 token.html，未必有用
2. qx 配置抓token，可以抓网页:[价格保护](https://msitepp-fm.jd.com/rest/priceprophone/priceProPhoneMenu)或者APP，刷新一次获取一个Token

```
[rewrite_local]
https:\/\/api\.m.jd.com\/api\?appid=siteppM&functionId=siteppM_priceskusPull url script-request-body https://raw.githubusercontent.com/ZCY01/daily_scripts/main/jd/jd_priceProtectRewrite.js
```

nodes 配置token：JD_TOKENS，token之间以 `@` 分隔，配置任意个token均可
