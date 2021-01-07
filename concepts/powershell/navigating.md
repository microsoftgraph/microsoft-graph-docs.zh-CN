---
title: 导航 Microsoft Graph PowerShell SDK
description: Microsoft Graph PowerShell SDK 包含大量命令。 了解如何找到适用于要实现的目标的命令。
localization_priority: Normal
author: jasonjoh
ms.openlocfilehash: 79c5ce415d00ba63ed6007e21248d51e721035c4
ms.sourcegitcommit: 7732d20bd99a125118f7cea146c3f2416879f949
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/07/2021
ms.locfileid: "49777587"
---
# <a name="navigating-the-microsoft-graph-powershell-sdk"></a>导航 Microsoft Graph PowerShell SDK

Microsoft Graph API 是一个巨大且不断增长的 API。 因此，Microsoft Graph PowerShell SDK 中的命令数量也非常大。 找到想要实现的目标正确的命令可能非常困难，尤其是在你尚未熟悉 Microsoft Graph 时。 让我们看一下一些有助于查找特定命令的方法。

## <a name="command-naming-conventions"></a>命令命名约定

SDK 中的命令直接从 [REST API](/graph/api/overview?view=graph-rest-1.0&preserve-view=true)生成，因此名称受 API 影响。 使用此 SDK 不需要了解 API 的详细信息，但这有助于了解命名约定。

PowerShell 命令使用动词名词对命名，例如 `Get-Command` 或 `Update-List` 。 让我们从动词开始。

### <a name="command-verbs"></a>命令动词

对于基本 REST 操作，动词由用于 API 的 HTTP 方法确定。

| HTTP 方法 | 命令动词 | 示例 |
|-------------|--------------|---|
| GET         | 获取          | `Get-MgUser` [API 参考](/graph/api/user-get?view=graph-rest-1.0&preserve-view=true) |
| POST        | 新式          | `New-MgUserMessage` [API 参考](/graph/api/user-post-messages?view=graph-rest-1.0&preserve-view=true) |
| PUT         | 新式          | `New-MgTeam` [API 参考](/graph/api/team-put-teams?view=graph-rest-1.0&preserve-view=true) |
| PATCH       | 更新       | `Update-MgUserEvent` [API 参考](/graph/api/event-update?view=graph-rest-1.0&preserve-view=true) |
| DELETE      | 删除       | `Remove-MgDriveItem` [API 参考](/graph/api/driveitem-delete?view=graph-rest-1.0&preserve-view=true) |

对于函数和操作，这有点复杂。 在 Microsoft Graph 中作为 OData 函数或操作实现的 API 通常使用至少一个动词进行命名。 相应的命令的动作基于函数或操作名称中的动词。 但是，PowerShell 中的命令动作必须符合特定的命名规则，[](/powershell/scripting/developer/cmdlet/approved-verbs-for-windows-powershell-commands)因此这可能会导致名称到命令的映射不直观。

让我们看一些示例。 [getSchedule](/graph/api/calendar-getschedule?view=graph-rest-1.0&preserve-view=true) API 使用 `get` ，并且是 `Get` 一个已批准的 PowerShell 动词，因此它的命令是 `Get-MgUserCalendarSchedule` 。 另 [一](/graph/api/event-cancel?view=graph-rest-beta&preserve-view=true) 方面，事件的取消 API 使用未批准的动词 `cancel` 。 用于取消或中断某些内容的批准动词是， `Stop` 因此它的命令为 `Stop-MgUserEvent` 。 最后 [，snoozeReminder](/graph/api/event-snoozereminder?view=graph-rest-1.0&preserve-view=true) API 的动词没有 `snooze` 经 PowerShell 批准的等效项。 对于 API，SDK 使用动词， `Invoke` 以便 API 的命令为 `Invoke-MgSnoozeUserEventReminder` 。

### <a name="command-nouns"></a>命令名词

至此，您可能已注意到 SDK 命令中所有名词以开始 `Mg` 。 此前缀有助于避免与其他 PowerShell 模块的命名冲突。 因此，使用类似命令获取 `Get-MgUser` 用户应该很有意义。 遵循 PowerShell 约定，即使名词是单数，如果没有请求特定实例，这些相同的命令也可以返回多个结果。

但是，类似或这样的 `Get-MgUserMessage` 命令呢 `Get-MgUserMailFolderMessage` ？ 这两者都获取 [一个消息](/graph/api/resources/message?view=graph-rest-1.0&preserve-view=true) 对象，那么为什么不 `Get-MgMessage` 呢？ 答案来自获取消息[API。](/graph/api/message-get?view=graph-rest-1.0&preserve-view=true)

查看此 API 的 HTTP 请求。 忽略 URL 中的请求， `/me` 还有两种调用此 API 的其他方法。

```http
GET /users/{id | userPrincipalName}/messages/{id}
GET /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}
```

路径与名词匹配。 对于第一个窗体，您以 `users` ，then 开始 `messages` ，因此该命令为 `Get-MgUserMessage` 。 第二个窗体中，首先为 `users` ，然后 `mailFolders` 是消息，因此命令为 `Get-MgUserMailFolderMessage` 。

查看此内容的另一种方式是拥有或包含的内容。 用户拥有邮件文件夹，邮件文件夹包含邮件。 添加前缀，然后获取 `Get-MgUserMailFolderMessage` 。

### <a name="listing-parameters"></a>列出参数

找到正确的命令后，可以使用该命令检查所有可用 `Get-Help` 参数。 例如，以下命令列出了该命令的所有可用 `Get-MgUser` 参数。

```powershell
Get-Help Get-MgUser -Detailed
```

## <a name="finding-available-commands"></a>查找可用命令

有时，仅知道命名约定不足以猜测正确的命令。 在这种情况下，可以使用该命令搜索 SDK `Get-Command` 中的可用命令。 例如，如果要查找与 Microsoft Teams 相关的命令，可以运行以下命令。

```powershell
Get-Command -Module Microsoft.Graph* *team*
```
