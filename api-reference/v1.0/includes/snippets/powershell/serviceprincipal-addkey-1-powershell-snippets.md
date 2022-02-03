---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 35776ab89be833509d5e4c090d6f77f9a13dfb76
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346640"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    KeyCredential = @{
        Type = "AsymmetricX509Cert"
        Usage = "Verify"
        Key = [System.Text.Encoding]::ASCII.GetBytes("MIIDYDCCAki...")
    }
    PasswordCredential = $null
    Proof = "eyJ0eXAiOiJ..."
}

Add-MgServicePrincipalKey -ServicePrincipalId $servicePrincipalId -BodyParameter $params

```