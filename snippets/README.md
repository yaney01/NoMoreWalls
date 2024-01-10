# 配置片段

这里存放了一些从 `list.yml` 中拆分出的配置片段，用于将本项目提供的一些配置整合到其它配置中。

# 文件说明

## Proxy Providers 规则集

- [nodes.yml](./nodes.yml)：节点列表，注意**不要**和下文的 `proxy.yml` 搞混了。
- [nodes_redir.yml](./nodes_redir.yml)：中转节点列表。
- nodes_地区码.yml：相应地区的节点列表，根据名称识别，不保证准确性，也不保证使用第三方服务时是否会被判断为国区。

## Rule Providers 规则集

- [adblock.yml](./adblock.yml)：广告屏蔽域名列表。
- [proxy.yml](./proxy.yml)：需要走代理的域名列表。
- [direct.yml](./direct.yml)：需要直连的域名列表。
- [region.yml](./region.yml)：存在锁区的域名列表。

注意：广告拦截列表中的域名不会出现在需要走代理的域名列表中，因此即使您没有使用广告屏蔽规则，仍有一些广告会无法加载。
