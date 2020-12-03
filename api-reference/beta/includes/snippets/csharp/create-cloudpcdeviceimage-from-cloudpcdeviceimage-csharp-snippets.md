---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: af24c2069eabe790378ea40ae5ce324b92016739
ms.sourcegitcommit: 9f88b7e41a4a4a4d5f52bd995ce07c6f702bd5d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/01/2020
ms.locfileid: "49523573"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var cloudPcDeviceImage = new CloudPcDeviceImage
{
    DisplayName = "Display Name value",
    OsBuildNumber = "OS Build Number value",
    OperatingSystem = "Operating System value",
    Version = "Version value",
    SourceImageResourceId = "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/Example/providers/Microsoft.Compute/images/exampleImage"
};

await graphClient.DeviceManagement.VirtualEndpoint.DeviceImages
    .Request()
    .AddAsync(cloudPcDeviceImage);

```