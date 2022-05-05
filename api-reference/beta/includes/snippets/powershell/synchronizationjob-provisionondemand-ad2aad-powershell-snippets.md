---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aa2e53806cde76d4522fbd9e2191f3d5d3713c4c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202904"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Parameters = @(
        @{
            RuleId = "6c409270-f78a-4bc6-af23-7cf3ab6482fe"
            Subjects = @(
                @{
                    ObjectId = "CN=AdeleV,CN=Users,DC=corp,DC=chicago,DC=com"
                    ObjectTypeName = "user"
                }
            )
        }
    )
}

New-MgServicePrincipalSynchronizationJobOnDemand -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```