---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b0bb4bf519de58e61d1071ab4db112ebf0f7a05c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62095263"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    OriginalStartTimeZone = "originalStartTimeZone-value"
    OriginalEndTimeZone = "originalEndTimeZone-value"
    ICalUId = "iCalUId-value"
    ReminderMinutesBeforeStart = 
    IsReminderOn = $true
}

Update-MgGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```