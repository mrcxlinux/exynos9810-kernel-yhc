# DS-萤火虫内核适用于 Exynos9810

这是我第一次处理内核，请不要嘲笑。仅在使用 Project Startlet（OneUI 6.1）的 Starlte 上测试过，理论上适用于其他设备，但不保证。我也将脚本翻译成了中文。

从 Duhan 的 Exynos9810 Apollo 内核分叉而来
## 编译
#### 方法 1：在你的机器上手动编译

仅在 Deepin 上测试过，但应该适用于任何基于 Debian/Ubuntu 的发行版。

```bash
 git clone https://github.com/mrcxlinux/exynos9810-kernel-yhc
 cd exynos9810-kernel-yhc
 ./apollo.sh
```
#### 方法 2：GitHub Actions（WIP）
叉（fork）这个仓库，然后转到“Actions”标签页，选择“Compile kernel”，点击“Run workflow”，按照指示操作，然后再次点击“Run workflow”。

此方法目前不稳定，因此不推荐使用，因为在你自己的机器上编译可能会更快且更容易调试。然而，如果你希望跟上我们的提交，同时避免不断开启和操作计算机的麻烦，你可以尝试这个方法。

如果你的分叉工作流因工作流错误而失败，请转到方法 1 进行编译，并将任何问题报告给我们。我们会尽力协助解决遇到的问题。

## 安装
只需将 IMG 文件刷入“boot”分区，或在 TWRP 中刷入 ZIP 文件。

## 真诚的感谢

- [@ananjaser1211](https://https://github.com/ananjaser1211)
- [@duhansysl](https://github.com/duhansysl)
- [@Florine0928](https://www.github.com/Florine0928)
- [@ExtremeXT](https://github.com/ExtremeXT)
