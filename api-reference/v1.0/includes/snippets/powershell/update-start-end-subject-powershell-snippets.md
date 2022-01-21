---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 64d0b4848942381abaa3261bb38e0f72b4f5f0e0
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136002"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    StartDateTime = [System.DateTime]::Parse("2020-09-09T14:33:30.8546353-07:00")
    EndDateTime = [System.DateTime]::Parse("2020-09-09T15:03:30.8566356-07:00")
    Subject = "Patch Meeting Subject"
}

Update-MgUserOnlineMeeting -UserId $userId -OnlineMeetingId $onlineMeetingId -BodyParameter $params

```