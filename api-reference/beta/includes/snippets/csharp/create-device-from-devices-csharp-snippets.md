---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8f8590cee319abc3bce022d12e54eb6a7dfa8a8
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61023973"
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
            Key = Convert.FromBase64String("base64Y3YxN2E1MWFlYw==")
        }
    },
    ApproximateLastSignInDateTime = DateTimeOffset.Parse("2016-10-19T10:37:00Z"),
    DeviceId = "deviceId-value",
    DeviceMetadata = "deviceMetadata-value",
    DeviceVersion = 99
};

await graphClient.Devices
    .Request()
    .AddAsync(device);

```