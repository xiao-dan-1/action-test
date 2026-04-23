# 🚀 自动化实验室：全功能组件测试

欢迎来到全功能展示页面。这篇文章包含了 Markdown 的各种高级语法，用来检验 MkDocs Material 主题在“极简”背后的强大渲染力。

---

## 1. 优雅的排版与引用

在网络工程的世界里，**“正确的前提下，极简优雅”** 是我们的最高指导原则。我们可以使用*斜体*来强调语气，或者使用~~删除线~~来标记过时的技术。

> **架构师语录：**
>
> 任何可以通过代码自动化的流程，都不应该让人工去点击第二次。这就是 CI/CD 存在的意义。

## 2. 极客代码块 (带行号与高亮)

得益于我们在配置中开启的 `pymdownx.highlight` 插件，代码块现在不仅支持精准的语法高亮，还带有行号，右上角还会自动生成“一键复制”按钮。

**Python 自动化脚本示例：**
```python
def deploy_blog(is_elegant: bool):
    """
    一个极简的部署逻辑演示
    """
    if is_elegant:
        print("🚀 Using GitHub Actions Artifacts...")
        return "Success!"
    else:
        raise Exception("Configuration is not minimal enough!")
```

**Linux 终端命令示例：**
```bash
# 获取本机的 IPv6 出口地址
curl -s -6 [https://ifconfig.co](https://ifconfig.co)

# 检查 OpenWrt 路由表
ip -6 route show
```

## 3. 任务清单 (Task Lists)

使用任务清单可以清晰地追踪项目的进度。这也是 GitHub 原生极力推荐的格式：

- [x] 搞懂 GitHub Actions 的三大核心组件
- [x] 成功部署基础版 MkDocs 博客
- [x] 实现 `mkdocs.yml` 与 `mkdocs-advanced.yml` 的优雅共存
- [ ] 开发一个定时检测内网 IPv6 状态的爬虫机器人

## 4. 数据表格 (Tables)

在对比不同技术方案时，表格是最直观的展现形式：

| 部署方案                       |  触发方式  | 状态隔离 |   优雅度评估   |
| :----------------------------- | :--------: | :------: | :------------: |
| 传统 FTP 上传                  |    手动    |   极差   |   ❌ 原始时代   |
| 推送至 `gh-pages` 脏分支       |   `push`   |   一般   |   ⚠️ 勉强及格   |
| **Actions Artifacts 内存打包** | **`push`** | **完美** | **✅ 极简优雅** |

## 5. 高级警告提示框 (Admonitions)

这是 Material 主题最标志性的功能！它可以让枯燥的文档瞬间拥有极高的辨识度。

!!! tip "运维小贴士"
    在配置 Cloudflare Zero Trust 时，请确保你的 WARP 客户端始终保持在最新版本，以获得最稳定的连接。

!!! warning "配置警告"
    修改 OpenWrt 的防火墙规则前，务必备份 `/etc/config/firewall` 文件。

!!! danger "绝对红线"
    无论在什么情况下，都**绝对不要**把你的服务器 SSH 私钥 (Private Key) 直接明文写在公开的 GitHub 仓库里！请务必使用 Actions Secrets。

## 6. 可折叠详情框 (Details 插件)

如果你有大段的辅助信息或冗长的日志，不要让它们占据主屏幕，把它们藏起来：

??? note "点击展开：查看详细的诊断日志"
    ```text
    [INFO] Fetching origin...
    [INFO] Analyzing branch 'main'
    [WARNING] Skipped 3 unused variables.
    [SUCCESS] Deployment completely elegant.
    ```

???+ warning "这是一个默认处于打开状态的折叠框"
    注意看开头的符号是 `???+`。它默认展开，但你可以点击标题把它收纳起来，非常适合放长篇的前置声明。

## 7. 外部片段注入 (Snippets 插件)

这是极客最爱的魔法！下面这个代码块**并没有写在这篇 Markdown 里**，而是 Actions 在云端编译时，像剪刀一样自动从 `snippets/ipv6_check.sh` 文件里“剪切”过来的。

**源文件永远同步，告别复制粘贴：**

```bash
--8<-- "docs/snippets/ipv6_check.sh"
```
