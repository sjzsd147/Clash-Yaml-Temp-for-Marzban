# Clash YAML Template for Marzban

专为 [Marzban](https://github.com/Gozargah/Marzban) 面板打造的专业 Clash 订阅配置模板。基于业内顶级的 [blackmatrix7 规则库](https://github.com/blackmatrix7/ios_rule_script)，为您和您的用户提供开箱即用、丝滑流畅的网络分流体验。

## 📖 一键部署

请通过 SSH 登录到您的 Marzban 服务器，依次执行以下命令：

1. **下载配置模板**
```bash
mkdir -p /var/lib/marzban/templates/clash
wget -O /var/lib/marzban/templates/clash/default.yml https://raw.githubusercontent.com/sjzsd147/Clash-Yaml-Temp-for-Marzban/main/default.yml
```

2. **修改 Marzban 环境变量**
```bash
echo "CLASH_SUBSCRIPTION_TEMPLATE=/var/lib/marzban/templates/clash/default.yml" >> /opt/marzban/.env
```

3. **重启面板生效**
```bash
marzban restart
```

客户端更新订阅后即可生效。

## 📜 鸣谢

* [Marzban](https://github.com/Gozargah/Marzban)
* [blackmatrix7 / ios_rule_script](https://github.com/blackmatrix7/ios_rule_script)
