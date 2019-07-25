---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 73811234dfe2f8b956f99007f8be1946b722e74f
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35713430"
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