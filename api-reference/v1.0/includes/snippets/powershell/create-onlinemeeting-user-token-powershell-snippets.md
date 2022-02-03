---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 06b0c9522b71fd23c18844754a148efb8630daaa
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350256"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    StartDateTime = [System.DateTime]::Parse("2019-07-12T14:30:34.2444915-07:00")
    EndDateTime = [System.DateTime]::Parse("2019-07-12T15:00:34.2464912-07:00")
    Subject = "User Token Meeting"
}

# A UPN can also be used as -UserId.
New-MgUserOnlineMeeting -UserId $userId -BodyParameter $params

```