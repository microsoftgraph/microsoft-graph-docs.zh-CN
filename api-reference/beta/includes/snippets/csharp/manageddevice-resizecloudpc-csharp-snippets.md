---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76050f9274218ce9add79a36273f50b6692bc2c9
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61525888"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var targetServicePlanId = "30d0e128-de93-41dc-89ec-33d84bb662a0";

await graphClient.DeviceManagement.ManagedDevices["{managedDevice-id}"]
    .ResizeCloudPc(targetServicePlanId)
    .Request()
    .PostAsync();

```