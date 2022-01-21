---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bfb2caeb2130245fbf1666107565bf27474cf237
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115532"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Action = "alert"
    ActivityGroupNames = @(
    )
    Confidence = 0
    Description = "This is a canary indicator for demo purpose. Take no action on any observables set in this indicator."
    ExpirationDateTime = [System.DateTime]::Parse("2019-03-01T21:43:37.5031462+00:00")
    ExternalId = "Test--8586509942679764298MS501"
    FileHashType = "sha256"
    FileHashValue = "aa64428647b57bf51524d1756b2ed746e5a3f31b67cf7fe5b5d8a9daf07ca313"
    KillChain = @(
    )
    MalwareFamilyNames = @(
    )
    Severity = 0
    Tags = @(
    )
    TargetProduct = "Azure Sentinel"
    ThreatType = "WatchList"
    TlpLevel = "green"
}

New-MgSecurityTiIndicator -BodyParameter $params

```