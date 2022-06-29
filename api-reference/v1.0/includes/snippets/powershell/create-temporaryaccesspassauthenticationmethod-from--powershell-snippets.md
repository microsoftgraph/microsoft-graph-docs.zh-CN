---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7fc1faf2610db50b99f359819035a2fcbcf82935
ms.sourcegitcommit: b2b3c3ae00f9e2e0bb2dcff30e97b60ccdebf170
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/29/2022
ms.locfileid: "66438524"
---
```powershell

Import-Module Microsoft.Graph.Identity.SignIns

$params = @{
    StartDateTime = [System.DateTime]::Parse("2022-06-05T00:00:00.000Z")
    LifetimeInMinutes = 60
    IsUsableOnce = $false
}

New-MgUserAuthenticationTemporaryAccessPassMethod -UserId $userId -BodyParameter $params

```