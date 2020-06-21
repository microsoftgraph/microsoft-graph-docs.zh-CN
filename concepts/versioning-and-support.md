---
title: 'Microsoft Graph 的版本控制、支持和重大更改策略 '
description: 本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。
localization_priority: Priority
ms.openlocfilehash: 47d0ec66fc335a50826d94511c8f9e6551c927a6
ms.sourcegitcommit: 3c8a92d89ac60a48cb63449976b1c3c2c6302281
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/16/2020
ms.locfileid: "44744003"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Microsoft Graph 的版本控制、支持和中断性变更策略

本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。

## <a name="support-policy-and-deprecation-information"></a>支持策略和弃用信息

Microsoft Graph 遵循 [Microsoft 生命周期策略](https://support.microsoft.com/lifecycle)。

As new versions of the Microsoft Graph REST APIs and Microsoft Graph SDKs are released, earlier versions will be retired. Microsoft will declare a version as deprecated at least 24 months in advance of retiring an API or an SDK.

递增 API 的主要版本（例如，从 v1.0 到 v2.0）时，我们将通知立即弃用当前版本（在此示例中为 v1.0），在通知 24 个月后，我们将不再支持该版本。 出于服务安全或运行状况可靠性问题的考虑，我们可能会对此策略作例外处理。

当 API 被标记为已弃用时，我们强烈建议你尽快迁移到最新版本。 某些情况下，我们将公布新应用程序必须在原始 API 弃用后不久开始使用新的 API。 在这些情况下，仅当前使用已弃用 API 的活动应用程序能够继续使用它们。

### <a name="api-contract-and-non-backward-compatible-changes"></a>API 协定和非后向兼容更改

Microsoft Graph has a log of changes across versions. These changes are listed in the [Microsoft Graph Changelog](changelog.md). As new functionality and data is added to Microsoft Graph, we will increment the API version number for any non-backward compatible changes to the API.

非后向兼容更改的示例如下：

- 对与资源关联的 URL 或基本请求/响应进行更改
- 删除、重命名或更改声明的属性的类型
- 删除或重命名 API 或 API 参数
- 添加所需的请求标头

向后兼容的更改示例如下：

- 添加可为 Null 或具有默认值的属性
- 向枚举添加成员
- 删除、重命名或更改开放扩展的类型
- 删除、重命名或更改注释的类型
- 向现有集合引入分页
- 更改错误代码
- 更改属性的顺序
- 更改不透明字符串（如资源 ID）的长度或格式

>**Note:** Over time, we will update the list of backward compatible changes. If you generate your own client proxies (like WCF clients), our guidance is that your client applications should be prepared to receive properties and derived types not previously defined by the Microsoft Graph API service. Microsoft Graph API follows the guidance described in the [Model Versioning](https://github.com/Microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning) section in the [Microsoft REST API guidelines](https://github.com/microsoft/api-guidelines/).

## <a name="versions"></a>版本

以下版本的 Microsoft Graph API 目前可用。

### <a name="beta-version"></a>Beta 版
Microsoft Graph API beta 版在 `https://graph.microsoft.com/beta` 中公开，包含当前_**处于预览状态**_ 的功能。 如需了解 beta API 文档，请参阅 [Microsoft Graph beta 终结点参考](/graph/api/overview?view=graph-rest-beta)。 预计将不时地对 beta 版本进行重大更改。 请勿对 /beta API 产生生产依赖性。

We make no guarantees that a beta feature will be promoted to the current version. When the Microsoft Graph API team believes that a beta feature is ready for general availability (GA), we will add that feature to the latest current version. If the promotion of the feature would result in a breaking change to the current version, the version number will be incremented, with the new version becoming the current version.
Our developer community can post feature request on [UserVoice](https://officespdev.uservoice.com/), including requests for new features as well as requests to promote existing beta APIs to the current version.

### <a name="current-version"></a>当前版本

The current version of Microsoft Graph is v1.0. Exposed under `https://graph.microsoft.com/v1.0`, the Microsoft Graph API /v1.0 version contains features that are generally available and ready for production use. You can browse the documentation for the v1.0 APIs in the table of contents.

### <a name="deprecated-and-unsupported-versions"></a>已弃用和不支持的版本

目前没有弃用的 Microsoft Graph 版本。

## <a name="terms-of-use"></a>使用条款

使用 Microsoft Graph API 即表示你同意 [Microsoft API 使用条款](/legal/microsoft-apis/terms-of-use?context=/graph/context)。

Your feedback is important to us. Connect with us on [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest). Tag your questions with [microsoft-graph].
