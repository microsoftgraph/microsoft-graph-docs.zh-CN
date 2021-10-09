---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 36f1681d7046dacef62314a4712fdab789770b2904435539a2055ecf28d294b9
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161346"
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