---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 10145a8fda77acf66d896889e56d9c7a59bb194f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34470344"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    AccountEnabled = false,
    AlternativeSecurityIds = new List<AlternativeSecurityId>()
    {
        new AlternativeSecurityId
        {
            Type = 2,
            Key = "base64Y3YxN2E1MWFlYw=="
        }
    },
    DeviceId = "4c299165-6e8f-4b45-a5ba-c5d250a707ff",
    DisplayName = "Test device",
    OperatingSystem = "linux",
    OperatingSystemVersion = "1"
};

await graphClient.Devices
    .Request()
    .AddAsync(device);

```