---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0426add71eef9d40788728557f020718efc5664
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62115210"
---
```powershell

Import-Module Microsoft.Graph.WindowsUpdates

$params = @{
    "@odata.type" = "#microsoft.graph.windowsUpdates.deployment"
    Content = @{
        "@odata.type" = "microsoft.graph.windowsUpdates.featureUpdateReference"
        Version = "20H2"
    }
    Settings = @{
        "@odata.type" = "microsoft.graph.windowsUpdates.windowsDeploymentSettings"
        Rollout = @{
            DevicesPerOffer = 100
        }
        Monitoring = @{
            MonitoringRules = @(
                @{
                    "@odata.type" = "#microsoft.graph.windowsUpdates.monitoringRule"
                    Signal = "rollback"
                    Threshold = 5
                    Action = "pauseDeployment"
                }
            )
        }
    }
}

New-MgWindowsUpdatesDeployment -BodyParameter $params

```