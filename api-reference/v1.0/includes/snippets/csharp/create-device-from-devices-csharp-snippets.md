---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b5c84e9ba8edfca76948449b1beebf31e1edda7c069a22b8d93fa7b3f07b702a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333523"
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