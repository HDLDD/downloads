# 安装包发布仓库

这个仓库只放 **Release 资产**（APK 等安装包），不放源码 —— 源码在各产品自己的仓库里。

| 产品 | 仓库 | 下载页 |
|---|---|---|
| NativeThink（英语思维训练） | [HDLDD/NativeThink](https://github.com/HDLDD/NativeThink) | https://nativethink-dl.pages.dev/ |
| CetExam（四六级备考） | — | 同上 |

每个版本一个 Release，资产名带版本号（如 `NativeThink-2.0.25.apk`），
对应 tag 形如 `nativethink-2.0.25`。Release 正文里写明体积与 SHA-256，
下载页的 `/dl/<app>/<platform>` 短链会 302 到这里的资产地址。

上传由 `nativethink-dl` 工程里的 `scripts/publish.mjs` 完成，不要手动往这里推文件。
