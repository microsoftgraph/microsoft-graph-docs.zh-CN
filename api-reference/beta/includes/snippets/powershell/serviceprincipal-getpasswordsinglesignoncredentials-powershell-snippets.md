---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 93738582f3e22e50f09f02f5246f53886b7d3cc1
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347474"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Id = "5793aa3b-cca9-4794-679a240f8b58"
}

Get-MgServicePrincipalPasswordSingleSignOnCredentials -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```