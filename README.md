### OpenWrt golang multi-branch

本仓库提供 3 个分支，分别跟踪不同 Go 版本线：

- `main` -> Go `1.24.x`（默认）
- `1.25` -> Go `1.25.x`
- `1.26` -> Go `1.26` 预发布（rc/beta）

`check-go-versions.yml` 会按分支自动检查并更新对应版本与 `PKG_HASH`。

### How to use 1.25.*

```shell
rm -rf feeds/packages/lang/golang
git clone https://github.com/kenzok8/golang -b 1.25 feeds/packages/lang/golang
```

### How to use 1.24.* (默认 / main)

```shell
rm -rf feeds/packages/lang/golang
git clone https://github.com/kenzok8/golang feeds/packages/lang/golang
```

### How to use 1.26.*

```shell
rm -rf feeds/packages/lang/golang
git clone https://github.com/kenzok8/golang -b 1.26 feeds/packages/lang/golang
```
