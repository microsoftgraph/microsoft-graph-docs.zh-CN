---
title: 导航 Microsoft Graph PowerShell SDK
description: Microsoft Graph PowerShell SDK 包含大量命令。 了解如何查找您想要实现的功能的正确命令。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: ceb4b0f783d1ad9a24cfc196d4099d5e67b3f273
ms.sourcegitcommit: b70ee16cdf24daaec923acc477b86dbf76f2422b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/22/2020
ms.locfileid: "48193658"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>导航 Microsoft Graph PowerShell SDK

Microsoft Graph API 非常大，现在都在不断增长。 因此，Microsoft Graph PowerShell SDK 中的命令数也非常大。 为要实现的内容找到正确的命令可能会非常困难，尤其是在您尚不熟悉 Microsoft Graph 的情况下。 让我们来看一些帮助查找特定命令的方法。

## <a name="command-naming-conventions"></a>命令命名约定

SDK 中的命令是直接从 [REST API](/graph/api/overview?view=graph-rest-1.0)生成的，因此这些名称受 API 影响。 您无需了解使用此 SDK 的 API 的详细信息，但有助于理解命名约定。

PowerShell 命令是使用动词-名词对（例如或）命名 `Get-Command` 的 `Update-List` 。 让我们从动词开始。

### <a name="command-verbs"></a>命令谓词

对于基本 REST 操作，谓词由用于 API 的 HTTP 方法决定。

| HTTP 方法 | 命令谓词 | 示例 |
|-------------|--------------|---|
| GET         | 获取          | `Get-MgUser` [API 参考](/graph/api/user-get?view=graph-rest-1.0) |
| POST        | 新式          | `New-MgUserMessage` [API 参考](/graph/api/user-post-messages?view=graph-rest-1.0) |
| PUT         | 新式          | `New-MgTeam` [API 参考](/graph/api/team-put-teams?view=graph-rest-1.0) |
| PATCH       | 更新       | `Update-MgUserEvent` [API 参考](/graph/api/event-update?view=graph-rest-1.0) |
| DELETE      | 删除       | `Remove-MgDriveItem` [API 参考](/graph/api/driveitem-delete?view=graph-rest-1.0) |

对于函数和操作，稍微复杂一些。 Microsoft Graph 中作为 OData 函数或操作实现的 Api 通常以至少一个谓词命名。 相应的命令谓词基于函数或操作名称中的谓词。 但是，PowerShell 中的命令谓词必须符合特定的 [命名规则](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)，因此这可能导致不直观的名称到命令映射。

我们来看一些示例。 [GetSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0) API 使用 `get` ，并且 `Get` 是已批准的 PowerShell 谓词，因此它的命令是 `Get-MgUserCalendarSchedule` 。 另一方面，在事件上的 [取消](/graph/api/event-cancel?view=graph-rest-beta) API 使用未经批准的谓词 `cancel` 。 "取消" 或 "不再" 的批准动词是 `Stop` ，因此它的命令是 `Stop-MgUserEvent` 。 最后， [snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0) API 的动词 `snooze` 没有经过 PowerShell 批准的等效项。 对于 API 这样的 API，SDK 使用动词 `Invoke` ，因此 api 的命令是 `Invoke-MgSnoozeUserEventReminder` 。

### <a name="command-nouns"></a>命令名词

到目前为止，你可能已注意到 SDK 的命令中的所有名词都以开头 `Mg` 。 此前缀有助于避免与其他 PowerShell 模块发生命名冲突。 明确这一点后， `Get-MgUser` 使用类似于获取用户的命令将会有意义。 和以下 PowerShell 约定（尽管名词是单数形式），如果没有请求特定的实例，则这些相同的命令可能会返回多个结果。

但像或这样的命令呢 `Get-MgUserMessage` `Get-MgUserMailFolderMessage` ？ 这两个类都将获取 [message](/graph/api/resources/message?view=graph-rest-1.0) 对象，因此为什么不会这么 `Get-MgMessage` 做呢？ 答案来自 [获取邮件 API](/graph/api/message-get?view=graph-rest-1.0)。

查看此 API 的 HTTP 请求。 忽略 `/me` URL 中的请求，有两种其他方法可调用此 API。

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

与名词匹配的路径。 对于第一个窗体，从开始 `users` ，然后 `messages` ，命令是 `Get-MgUserMessage` 。 在第二个窗体中，首先 `users` 是，然后 `mailFolders` 是邮件，因此命令是 `Get-MgUserMailFolderMessage` 。

查看此内容的另一种方法是拥有或包含哪些内容。 用户拥有邮件文件夹，邮件文件夹中包含邮件。 添加前缀并获取 `Get-MgUserMailFolderMessage` 。

## <a name="finding-available-commands"></a>查找可用命令

有时只知道命名约定并不能猜测正确的命令。 在这种情况下，可以使用 `Get-Command` 命令在 SDK 中搜索可用命令。 例如，如果您要查找与 Microsoft 团队相关的命令，则可以运行以下命令。

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
