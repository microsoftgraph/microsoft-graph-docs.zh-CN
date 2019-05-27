---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 73811234dfe2f8b956f99007f8be1946b722e74f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34453570"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var device = new Device
{
    AccountEnabled = true,
    AlternativeSecurityIds = new List<AlternativeSecurityId>()
    {
        new AlternativeSecurityId
        {
            Type = 99,
            IdentityProvider = "identityProvider-value",
            Key = "base64Y3YxN2E1MWFlYw=="
        }
    },
    ApproximateLastSignInDateTime = "2016-10-19T10:37:00Z",
    DeviceId = "deviceId-value",
    DeviceMetadata = "deviceMetadata-value",
    DeviceVersion = 99
};

await graphClient.Devices
    .Request()
    .AddAsync(device);

```