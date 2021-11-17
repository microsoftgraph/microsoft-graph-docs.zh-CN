---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8d507a6becec0084bfa8e11697e33109c0cb53c52f5e7eb3187b8d659e9d5aba
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var deployment = new Microsoft.Graph.WindowsUpdates.Deployment
{
    State = new DeploymentState
    {
        RequestedValue = Microsoft.Graph.WindowsUpdates.RequestedDeploymentStateValue.Paused
    }
};

await graphClient.Admin.Windows.Updates.Deployments["{windowsUpdates.deployment-id}"]
    .Request()
    .UpdateAsync(deployment);

```