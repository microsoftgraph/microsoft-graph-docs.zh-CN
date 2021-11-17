---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 426733b70ba5d3700e7f2d36c7343f5b75d6e3a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60974124"
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
            Key = Convert.FromBase64String("base64Y3YxN2E1MWFlYw==")
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