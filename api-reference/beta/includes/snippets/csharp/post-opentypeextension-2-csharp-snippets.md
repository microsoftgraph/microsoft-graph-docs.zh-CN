---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecd122b4dcfdcabaab2f6ff27a3fe0d11aa6d987
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792639"
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

await graphClient.Me.Messages["{message-id}"].Extensions
    .Request()
    .AddAsync(extension);

```