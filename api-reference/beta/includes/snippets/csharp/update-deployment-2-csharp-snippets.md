---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e9d3f01b2f76e650aa191e4413dbe0da136d8de4
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870288"
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