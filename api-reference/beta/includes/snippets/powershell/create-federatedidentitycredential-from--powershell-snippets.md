---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 22e1939e74f40a0e090e987a0f91540dd0c6cf0e
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62097273"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "testing02"
    Issuer = "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0"
    Subject = "a7d388c3-5e3f-4959-ac7d-786b3383006a"
    Audiences = @(
        "api://AzureADTokenExchange"
    )
}

New-MgApplicationFederatedIdentityCredential -ApplicationId $applicationId -BodyParameter $params

```