---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 16917dcaec5687c044d9b5fece83b64c53d1bd62
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62133557"
---
```powershell

Import-Module Microsoft.Graph.Groups

$params = @{
    OriginalStartTimeZone = "originalStartTimeZone-value"
    OriginalEndTimeZone = "originalEndTimeZone-value"
    Uid = "iCalUId-value"
    ReminderMinutesBeforeStart = 
    IsReminderOn = $true
}

Update-MgGroupThread -GroupId $groupId -ConversationThreadId $conversationThreadId -BodyParameter $params

```