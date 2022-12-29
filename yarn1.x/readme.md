- 重装 8ms
- .yarn-integrity文件，里面记录了依赖包的来源等











npm/yarn 本身还是存在扁平化算法复杂和package 非法访问的






脱离 node 生态
pnp 比较明显的缺点是脱离了 node 生态。

因为使用 PnP 不会再有 node_modules 了，但是 Webpack，Babel 等各种前端工具都依赖 node_modules。虽然很多工具比如 pnp-webpack-plugin 已经在解决了，但难免会有兼容性风险。
PnP 自建了依赖解析器，所有的依赖引用都必须由解析器执行，因此只能通过 yarn 命令来执行 node 脚本。