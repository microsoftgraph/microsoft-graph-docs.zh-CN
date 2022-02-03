---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 294a6db13c002eacd09edaf60f42f58765f2a4a6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62349862"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    StartDateTime = [System.DateTime]::Parse("2020-09-09T14:33:30.8546353-07:00")
    EndDateTime = [System.DateTime]::Parse("2020-09-09T15:03:30.8566356-07:00")
    Subject = "Patch Meeting Subject"
}

# A UPN can also be used as -UserId.
Update-MgUserOnlineMeeting -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```