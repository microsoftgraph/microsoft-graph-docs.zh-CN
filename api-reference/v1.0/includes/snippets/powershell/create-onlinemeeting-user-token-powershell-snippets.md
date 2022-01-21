---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 98d8fd3e27608b549ad89257de6071f3dfd2a204
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136504"
---
```powershell

Import-Module Microsoft.Graph.CloudCommunications

$params = @{
    StartDateTime = [System.DateTime]::Parse("2019-07-12T14:30:34.2444915-07:00")
    EndDateTime = [System.DateTime]::Parse("2019-07-12T15:00:34.2464912-07:00")
    Subject = "User Token Meeting"
}

New-MgUserOnlineMeeting -UserId $userId -BodyParameter $params

```