---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 66987f012a598ca22a2de20c5c57b91c13a758e6901a68eedab780263feafab5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57164311"
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