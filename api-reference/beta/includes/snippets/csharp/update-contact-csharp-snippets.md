---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4e725439a65b27492f7e9abbe4590b529d341e3d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35707507"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    EmailAddresses = new List<TypedEmailAddress>()
    {
        new TypedEmailAddress
        {
            Type = EmailType.Personal,
            Name = "Pavel Bansky",
            Address = "pavelb@adatum.onmicrosoft.com"
        },
        new TypedEmailAddress
        {
            Address = "pavelb@fabrikam.onmicrosoft.com",
            Name = "Pavel Bansky",
            Type = EmailType.Other,
            OtherLabel = "Volunteer work"
        }
    }
};

await graphClient.Me.Contacts["AAMkADh6v5AAAvgTCEAAA="]
    .Request()
    .UpdateAsync(contact);

```