---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a8eaf5628b438370565ac816b8adf57f3ce79d7a
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35463588"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityAction = new SecurityAction
{
    Name = "BlockIp",
    ActionReason = "Test",
    Parameters = new List<KeyValuePair>()
    {
        new KeyValuePair
        {
            Name = "IP",
            Value = "1.2.3.4"
        }
    },
    VendorInformation = new SecurityVendorInformation
    {
        Provider = "Windows Defender ATP",
        Vendor = "Microsoft"
    }
};

await graphClient.Security.SecurityActions
    .Request()
    .AddAsync(securityAction);

```