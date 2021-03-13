---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a7f4c173b1bb4f3d8406c1a4dd32ae9864a246d
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50807994"
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

await graphClient.Me.Contacts["{contact-id}"]
    .Request()
    .UpdateAsync(contact);

```