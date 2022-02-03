---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e775a06025f48032e9134166c0ccf6e9df82995
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62340470"
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

Add-MgApplicationKey -ApplicationId $applicationId -BodyParameter $params

```