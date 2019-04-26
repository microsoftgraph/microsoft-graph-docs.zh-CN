---
title: 'Microsoft Graph 的版本控制、支持和重大更改策略 '
description: 本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。
localization_priority: Priority
ms.openlocfilehash: 273772aaf72031ca27801e54ede744960c601fd4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575735"
---
# <a name="versioning-support-and-breaking-change-policies-for-microsoft-graph"></a>Microsoft Graph 的版本控制、支持和中断性变更策略 

本文介绍了 Microsoft Graph 的支持和重大更改策略，以及当前可用的 Microsoft Graph API 版本。

## <a name="support-policy-and-deprecation-information"></a>支持策略和弃用信息

Microsoft Graph 遵循 [Microsoft 生命周期策略](https://support.microsoft.com/zh-CN/lifecycle)。 

由于已发布新版本的 Microsoft Graph REST API 和 Microsoft Graph SDK，之前的版本将停用。Microsoft 将在停用 API 或 SDK 之前至少 24 个月声明弃用的版本。 

递增 API 的主要版本（例如，从 v1.0 到 v2.0）时，我们将通知立即弃用当前版本（在此示例中为 v1.0），在通知 24 个月后，我们将不再支持该版本。 出于服务安全或运行状况可靠性问题的考虑，我们可能会对此策略作例外处理。  

当 API 被标记为已弃用时，我们强烈建议你尽快迁移到最新版本。 某些情况下，我们将公布新应用程序必须在原始 API 弃用后不久开始使用新的 API。 在这些情况下，仅当前使用已弃用 API 的活动应用程序能够继续使用它们。   

### <a name="api-contract-and-non-backward-compatible-changes"></a>API 协定和非后向兼容更改

Microsoft Graph 在版本中进行了许多更改。这些更改已在 [Microsoft Graph 更改日志](changelog.md)中列出。随着向 Microsoft Graph 中添加新功能和数据，我们将递增 API 版本号，以对 API 进行任意不向后兼容更改。 

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

>**注意：** 随着时间的推移，我们将更新向后兼容更改的列表。如果你生成了自己的客户端代理（如 WCF 客户端），我们的建议是，客户端应用程序应准备接收之前未由 Microsoft Graph API 服务定义的属性和派生类型。Microsoft Graph API 遵循 [Microsoft REST API 准则](https://github.com/microsoft/api-guidelines/)的[模型版本控制](https://github.com/microsoft/api-guidelines/blob/master/Guidelines.md#12-versioning)部分中描述的指导。 

## <a name="versions"></a>版本

以下版本的 Microsoft Graph API 目前可用。

### <a name="beta-version"></a>Beta 版
Microsoft Graph API beta 版在 `https://graph.microsoft.com/beta` 中公开，包含当前_**处于预览状态**_ 的功能。 如需了解 beta API 文档，请参阅 [Microsoft Graph beta 终结点参考](/graph/api/overview?view=graph-rest-beta)。 预计将不时地对 beta 版本进行重大更改。 请勿对 /beta API 产生生产依赖性。

我们无法保证将测试功能升级至当前版本。当 Microsoft Graph API 团队认为测试功能可正式发布 (GA) 时，我们将把该功能添加到最新的当前版本中。如果功能升级将导致当前版本出现重大更改，则版本号将递增，而新版本将成为当前版本。我们的开发者社区可以在 [UserVoice](https://officespdev.uservoice.com/) 上发布功能请求，包括对新功能的请求以及将现有的测试 API 升级到当前版本的请求。 

### <a name="current-version"></a>当前版本

Microsoft Graph 的当前版本为 v1.0。Microsoft Graph API /v1.0 版本在 `https://graph.microsoft.com/v1.0` 中公开，包含可正式发布和可用于生产的功能。你可以浏览目录中的 v1.0 API 文档。

### <a name="deprecated-and-unsupported-versions"></a>已弃用和不支持的版本

目前没有弃用的 Microsoft Graph 版本。

## <a name="terms-of-use"></a>使用条款

使用 Microsoft Graph API，即表示同意接受[使用条款](https://developer.microsoft.com/graph/docs/misc/terms-of-use)。 

我们非常重视你的反馈意见。请在 [StackOverflow](https://stackoverflow.com/questions/tagged/microsoftgraph?sort=newest) 上与我们联系，并使用 [MicrosoftGraph] 为问题添加标签。
