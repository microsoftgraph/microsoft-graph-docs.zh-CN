---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ed3a23eca03ba50396d7972198d6dae553fe7b2c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62136399"
---
```powershell

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
    AccountEnabled = $false
    AlternativeSecurityIds = @(
        @{
            Type = 2
            Key = [System.Text.Encoding]::ASCII.GetBytes("base64Y3YxN2E1MWFlYw==")
        }
    )
    DeviceId = "4c299165-6e8f-4b45-a5ba-c5d250a707ff"
    DisplayName = "Test device"
    OperatingSystem = "linux"
    OperatingSystemVersion = "1"
}

New-MgDevice -BodyParameter $params

```