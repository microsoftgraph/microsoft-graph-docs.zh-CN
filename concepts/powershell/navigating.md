---
title: 导航 Microsoft Graph PowerShell SDK
description: Microsoft Graph PowerShell SDK 包含大量命令。 了解如何为要实现的目标找到正确的命令。
ms.localizationpriority: medium
author: jasonjoh
ms.openlocfilehash: 2c4135691712bcc6cbe8a32a776aa40844ec668e
ms.sourcegitcommit: 19558bd9de9b717e7a36bfce1d6d84d0132e2697
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/15/2022
ms.locfileid: "64883400"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>导航 Microsoft Graph PowerShell SDK

Microsoft 图形 API是巨大的，并且一直都在增长。 因此，Microsoft Graph PowerShell SDK 中的命令数也非常大。 找到适合你想要实现的命令可能会很有挑战性，尤其是在你尚不熟悉 Microsoft Graph的情况下。 我们来看看一些帮助查找特定命令的方法。

[!INCLUDE [aad-advanced-queries-note](../../includes/aad-advanced-queries-note.md)]

## <a name="command-naming-conventions"></a>命令命名约定

SDK 中的命令直接从 [REST API](/graph/api/overview?view=graph-rest-1.0&preserve-view=true) 生成，因此名称受 API 的影响。 无需了解使用此 SDK 的 API 的详细信息，但它有助于了解命名约定。

PowerShell 命令是使用谓词-名词对（例如 `Get-Command` 或 `Update-List`）命名的。 让我们从谓词开始。

### <a name="command-verbs"></a>命令谓词

对于基本 REST 操作，谓词由用于 API 的 HTTP 方法确定。

| HTTP 方法 | 命令谓词 | 示例 |
|-------------|--------------|---|
| GET         | 获取          | `Get-MgUser` [API 参考](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POST        | 新增          | `New-MgUserMessage` [API 参考](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | 新增          | `New-MgTeam` [API 参考](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | 更新       | `Update-MgUserEvent` [API 参考](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| DELETE      | 删除       | `Remove-MgDriveItem` [API 参考](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

对于函数和操作，这要复杂一些。 Microsoft Graph中作为 OData 函数或操作实现的 API 通常使用至少一个谓词进行命名。 相应命令的谓词基于函数或操作名称中的谓词。 但是，PowerShell 中的命令谓词必须符合特定 [的命名规则](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)，因此这可能导致非直观的名称到命令映射。

我们来看看一些示例。 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) API 使用`get`，并且`Get`是已批准的 PowerShell 谓词，因此它的命令是 `Get-MgUserCalendarSchedule`。 另一方面，事件上的 [取消](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) API 使用未经批准的谓词 `cancel`。 批准的谓词取消或停止某件东西是 `Stop`，所以命令是 `Stop-MgUserEvent`。 最后， [snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) API 的谓词 `snooze`没有 PowerShell 批准的等效项。 对于类似 API，SDK 使用谓词 `Invoke`，以便 API 的命令为 `Invoke-MgSnoozeUserEventReminder`。

### <a name="command-nouns"></a>命令名词

现在，你可能已经注意到，SDK 命令中的所有名词都是从 `Mg`开始的。 此前缀有助于避免与其他 PowerShell 模块的命名冲突。 考虑到这一点，使用类似 `Get-MgUser` 命令来获取用户应该很有意义。 按照 PowerShell 约定，即使名词是单一的，如果未请求任何特定实例，这些相同的命令也可以返回多个结果。

但是，命令的类似 `Get-MgUserMessage` 情况 `Get-MgUserMailFolderMessage`又如何呢？ 这两个都得到一个 [消息](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) 对象，那么为什么不 `Get-MgMessage`呢？ 答案来自 [获取消息 API](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true)。

查看此 API 的 HTTP 请求。 忽略 URL 中的请求 `/me` ，还有两种调用此 API 的方法。

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

路径与名词匹配。 对于第一个表单，首先 `users`是 `messages`命令 `Get-MgUserMessage`。 在第二种窗体中，首先 `users`是 `mailFolders`消息，所以命令是 `Get-MgUserMailFolderMessage`。

另一种查看方法是拥有或包含的内容。 用户拥有邮件文件夹，邮件文件夹包含邮件。 添加前缀并获取 `Get-MgUserMailFolderMessage`。

### <a name="listing-parameters"></a>列出参数

找到正确的命令后，可以使用 `Get-Help` 该命令检查所有可用参数。 例如，以下命令列出了该命令的所有可用参数 `Get-MgUser` 。

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>查找可用命令

有时，只知道命名约定不足以猜测正确的命令。 在这种情况下，可以使用该 `Get-Command` 命令搜索 SDK 中的可用命令。 例如，如果要查找与Microsoft Teams相关的命令，则可以运行以下命令。

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
