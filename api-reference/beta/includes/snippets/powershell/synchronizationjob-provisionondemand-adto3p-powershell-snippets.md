---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8e5ba65f5ca7713e876f985141bd66ce5254b30b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202905"
---
```powershell

Import-Module Microsoft.Graph.Applications

$params = @{
    Parameters = @(
        @{
            Subjects = @(
                @{
                    ObjectId = "9bb0f679-a883-4a6f-8260-35b491b8b8c8"
                    ObjectTypeName = "User"
                }
            )
            RuleId = "ea807875-5618-4f0a-9125-0b46a05298ca"
        }
    )
}

New-MgServicePrincipalSynchronizationJobOnDemand -ServicePrincipalId $servicePrincipalId -SynchronizationJobId $synchronizationJobId -BodyParameter $params

```