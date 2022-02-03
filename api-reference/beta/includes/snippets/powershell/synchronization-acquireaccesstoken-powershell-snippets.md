---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f3ab410f4844d6df26a4fa248fea9db8ecf391b
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62347072"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Credentials = @(
        @{
            "@odata.type" = "microsoft.graph.synchronizationSecretKeyStringValuePair"
        }
    )
}

Get-MgApplicationSynchronizationAccessToken -ApplicationId $applicationId -BodyParameter $params

```