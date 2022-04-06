---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f3e60bc244d0ee2993bbfad705e3cc9b7348d3d5
ms.sourcegitcommit: 0bcc0a93f37db6013be40dc8d36717aeeeef7fb6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/16/2022
ms.locfileid: "63528181"
---
```powershell

Import-Module Microsoft.Graph.Identity.Governance

$params = @{
    DisplayName = "Contoso ToU for guest users"
    IsViewingBeforeAcceptanceRequired = $true
    Files = @(
        @{
            FileName = "TOU.pdf"
            Language = "en"
            IsDefault = $true
            FileData = @{
                Data = [System.Text.Encoding]::ASCII.GetBytes("SGVsbG8gd29ybGQ=//truncated-binary")
            }
        }
    )
}

New-MgIdentityGovernanceTermOfUseAgreement -BodyParameter $params

```