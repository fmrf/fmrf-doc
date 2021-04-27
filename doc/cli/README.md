# fmrf-cli

胖蚊子兔场命令行工具.


## 命令目录

| 命令 | 说明 | 备注 |
| :--- | :-- | :--- |
| `fmrf host` | **主机命令** | 只能在主机 (如服务端树莓派) 设备上执行 |
| `fmrf host setup-check` | 安装检查 | 进行安装配置, 以及安装准备 |
| `fmrf host setup` | 执行安装 | 必须首先成功 `setup-check` |
| `fmrf host upgrade-check` | 升级检查 | 升级配置及准备 |
| `fmrf host upgrade` | 执行平滑升级 | 必须首先成功 `upgrade-check` |
| `fmrf host restart` | 系统重启 (启动) | 没有单独的启动命令 |
| `fmrf host shutdown` | 系统关闭 | |
| `fmrf host status` | 报告主机状态 | |
| `fmrf host user-add-pa` | 新增主管理员 (PA) 账号 | 系统默认不含任何账号, 必须手动添加 |
| `fmrf host user-first-login` | 账号首次登录 | 获取一次性登录证书及密钥 |
| `fmrf host ca-reset` | 重置 fmrf-ca 根证书 | 此操作会废弃之前所有生成的证书, 所有地方需要重新配置 |
| `fmrf ca` | **fmrf-ca 命令** | |
| `fmrf ca get-root-cert` | 获取根证书 | |
| `fmrf ca status` | 报告 CA 状态 | |
| `fmrf ha` | **高可用命令** | |
| `fmrf ha status` | 报告高可用状态 | |
| `fmrf global` | **全局操作命令** | |
| `fmrf global status` | 报告全局状态 | |
| `fmrf global lock` | 全局锁定 | 停止/禁用一切硬件设备操作 (现场所有设备停机) |
| `fmrf global unlock` | 全局解锁 | |
| `fmrf admin` | **管理员命令** | |
| `fmrf admin user-lock` | 锁定账号 | 锁定后的账号无法登录, 无法进行任何操作, 立即生效 |
| `fmrf admin user-unlock` | 解锁账号 | |
| `fmrf w` | **观察者命令** | |
| `fmrf login` | **登录命令** | |

TODO

## fmrf-cli 支持的平台

+ [`arm64v8`] 树莓派 4B (8GB 内存, 官方操作系统)

+ [`arm64v8`] Android (termux)

+ [`x86_64`] ArchLinux

+ [`x86_64`] Ubuntu

不支持的平台不会被测试, 且针对不支持的平台的 PR 不会被接受.


TODO
