# DNF90 客户端更新包

本仓库用于分发 DNF90 客户端的**增量更新包**。

## 下载

到 [Releases](../../releases) 页面下载最新版本。

## 说明

每个 Release 包含：

- `DNF90-client-<版本>-update.zip` —— 客户端文件（DNF.exe / Script.pvf / dstr.dat / ImagePacks2 部分 NPK）
- 包内 `SHA256SUMS.txt` —— 逐文件校验值
- 包内 `说明.txt` —— 使用步骤

## 用法

1. 下载并解压
2. 把文件覆盖到你的 DNF 客户端目录（含 `DNF.exe` 的那个目录）
3. 启动游戏

## 校验

```powershell
Get-FileHash DNF.exe -Algorithm SHA256
Get-FileHash Script.pvf -Algorithm SHA256
```

对比包内 `SHA256SUMS.txt`。

---

*资源来自上游官方渠道，哈希已逐一核对。*
