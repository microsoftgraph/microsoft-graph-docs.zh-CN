---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f93b3494b66be0fbb15630f4b1b1ee94b5d03118
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44685222"
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
            Key = Encoding.ASCII.GetBytes("base64Y3YxN2E1MWFlYw==")
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