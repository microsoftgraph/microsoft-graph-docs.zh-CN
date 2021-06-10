---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55682f3d2c2bc252c99e8e2a9ff4e9795e95dc49
ms.sourcegitcommit: 503c72036c376a30e08c29df8e7730a7afcab66e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2021
ms.locfileid: "52870302"
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