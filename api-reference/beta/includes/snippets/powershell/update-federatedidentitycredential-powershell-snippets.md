---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a3766f41fcfbb182af8bf7bb23877e8e5b2d459b
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62127867"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Name = "testing02"
    Issuer = "https://login.microsoftonline.com/3d1e2be9-a10a-4a0c-8380-7ce190f98ed9/v2.0"
    Subject = "a7d388c3-5e3f-4959-ac7d-786b3383006a"
    Description = "Updated description"
    Audiences = @(
        "api://AzureADTokenExchange"
    )
}

Update-MgApplicationFederatedIdentityCredential -ApplicationId $applicationId -FederatedIdentityCredentialId $federatedIdentityCredentialId -BodyParameter $params

```