---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a5800af671820f0c771aaf5f2cdbb677dfb84759
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62339368"
---
```powershell

Import-Module Microsoft.Graph.Security

$params = @{
    Value = @(
        @{
            AssignedTo = "String"
            ClosedDateTime = [System.DateTime]::Parse("String (timestamp)")
            Comments = @(
                "String"
            )
            Feedback = @{
                "@odata.type" = "microsoft.graph.alertFeedback"
            }
            Id = "String (identifier)"
            Status = @{
                "@odata.type" = "microsoft.graph.alertStatus"
            }
            Tags = @(
                "String"
            )
            VendorInformation = @{
                Provider = "String"
                Vendor = "String"
            }
        }
    )
}

Update-MgSecurityAlertMultiple -BodyParameter $params

```