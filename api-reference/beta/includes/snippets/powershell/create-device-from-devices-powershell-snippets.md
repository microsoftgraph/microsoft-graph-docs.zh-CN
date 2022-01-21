---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 58d4c9f43557549b62d51812458d65db0b4a6c99
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62103643"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    AccountEnabled = $true
    AlternativeSecurityIds = @(
        @{
            Type = 99
            IdentityProvider = "identityProvider-value"
            Key = [System.Text.Encoding]::ASCII.GetBytes("base64Y3YxN2E1MWFlYw==")
        }
    )
    ApproximateLastSignInDateTime = [System.DateTime]::Parse("2016-10-19T10:37:00Z")
    DeviceId = "deviceId-value"
    DeviceMetadata = "deviceMetadata-value"
    DeviceVersion = 99
}

New-MgDevice -BodyParameter $params

```