---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eb73d5a8d98a4dd367ca772e8df392addf5cb50a
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62343998"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    DisplayName = "CN=customDisplayName"
    EndDateTime = [System.DateTime]::Parse("2024-01-25T00:00:00Z")
}

Add-MgServicePrincipalTokenSigningCertificate -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```