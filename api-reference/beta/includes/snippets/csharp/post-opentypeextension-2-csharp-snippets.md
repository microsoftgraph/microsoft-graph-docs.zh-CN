---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5786deec5c0576c83e6f07f16e3b56bb8ea54efe
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684965"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var extension = new OpenTypeExtension
{
    ExtensionName = "Com.Contoso.Referral",
    AdditionalData = new Dictionary<string, object>()
    {
        {"companyName", "Wingtip Toys"},
        {"dealValue", "500050"},
        {"expirationDate", "2015-12-03T10:00:00Z"}
    }
};

await graphClient.Me.Messages["AAMkAGE1M2IyNGNmLTI5MTktNDUyZi1iOTVl==="].Extensions
    .Request()
    .AddAsync(extension);

```