# WeChatAidProxy

基于 [wechaty](https://github.com/wechaty/wechaty) 代理微信客户端，接入 MidJourney。

> ***微信代理有风险，使用需谨慎***

## 注意事项

- 依赖 [MidJourneyAidProxy]([Starry-Gaze/MidJourneyAidProxy: 代理 MidJourney 的discord频道，实现api形式调用AI绘图，公益项目 (github.com)](https://github.com/Starry-Gaze/MidJourneyAidProxy)) 提供的api接口
- 推荐使用docker启动；mac M或其他arm架构电脑，暂时使用npm启动

## npm启动

```shell
git clone git@github.com:Starry-Gaze/WeChatAidProxy.git
cd WeChatAidProxy
npm install
# 可能执行错误，缺少library，按提示解决
cp .env.example .env
# 更改配置项，启动服务
npm run serve
```

## 配置项

| 变量名            | 非空 | 描述                     |
| :---------------- | :--: | :----------------------- |
| MJ_PROXY_ENDPOINT |  是  | midjourney代理服务的地址 |
| BLOCK_WORDS       |  否  | 敏感词，英文逗号分隔     |

