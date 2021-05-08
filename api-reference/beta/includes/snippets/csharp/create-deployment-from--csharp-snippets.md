---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 361ea799792b29e904d356410da129d9143acbda
ms.sourcegitcommit: 2a35434fabc76672e21bfc3ed5a1d28f9f3b66bc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52239185"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployment = new Microsoft.Graph.WindowsUpdates.Deployment
{
    Content = new FeatureUpdateReference
    {
        Version = "20H2"
    },
    Settings = new WindowsDeploymentSettings
    {
        Rollout = new Microsoft.Graph.WindowsUpdates.RolloutSettings
        {
            DevicesPerOffer = 100
        },
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

await graphClient.Admin.Windows.Updates.Deployments
    .Request()
    .AddAsync(deployment);

```