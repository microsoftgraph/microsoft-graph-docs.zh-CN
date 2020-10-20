---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8eaf5628b438370565ac816b8adf57f3ce79d7a
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48609372"
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