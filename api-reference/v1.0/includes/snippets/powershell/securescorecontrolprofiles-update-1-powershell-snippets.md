---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 615ece547b432ae30f1cb0f67e964ececd494ba4
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62088082"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    AssignedTo = ""
    Comment = "control is reviewed"
    State = "Reviewed"
    VendorInformation = @{
        Provider = "SecureScore"
        ProviderVersion = $null
        SubProvider = $null
        Vendor = "Microsoft"
    }
}

Update-MgSecuritySecureScoreControlProfile -SecureScoreControlProfileId $secureScoreControlProfileId -BodyParameter $params

```