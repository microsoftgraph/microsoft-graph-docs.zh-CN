---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ae46c40dab3d60bac5ba3459d0139c371e676fd25044928732a7c640d4282e8d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279139"
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