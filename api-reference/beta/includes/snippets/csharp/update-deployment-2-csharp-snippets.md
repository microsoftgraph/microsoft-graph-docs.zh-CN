---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8216272a6185ee14c2c8acd5bc6e1e3636786bb75418ca5089ab457ac302196
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220472"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployment = new Microsoft.Graph.WindowsUpdates.Deployment
{
    Settings = new WindowsDeploymentSettings
    {
        Monitoring = new Microsoft.Graph.WindowsUpdates.MonitoringSettings
        {
            MonitoringRules = new List<Microsoft.Graph.WindowsUpdates.MonitoringRule>()
            {
                new Microsoft.Graph.WindowsUpdates.MonitoringRule
                {
                    Signal = Microsoft.Graph.WindowsUpdates.MonitoringSignal.Rollback,
                    Threshold = 5,
                    Action = Microsoft.Graph.WindowsUpdates.MonitoringAction.PauseDeployment
                }
            }
        }
    }
};

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"]
    .Request()
    .UpdateAsync(deployment);

```