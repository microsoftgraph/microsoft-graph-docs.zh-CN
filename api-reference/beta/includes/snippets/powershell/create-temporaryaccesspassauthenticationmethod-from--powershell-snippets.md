---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 28cd942819cc41e18912d726f0ffdce1505f7bb7
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62126747"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    "@odata.type" = "#microsoft.graph.temporaryAccessPassAuthenticationMethod"
    StartDateTime = [System.DateTime]::Parse("2021-01-26T00:00:00.000Z")
    LifetimeInMinutes = 60
    IsUsableOnce = $false
}

New-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId -BodyParameter $params

```