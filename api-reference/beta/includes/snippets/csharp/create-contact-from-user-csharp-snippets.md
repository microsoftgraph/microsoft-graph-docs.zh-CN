---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 588f5fd28ad7c86554b0167b8d7ef279689cc5fa
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35716369"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    GivenName = "Pavel",
    Surname = "Bansky",
    EmailAddresses = new List<TypedEmailAddress>()
    {
        new TypedEmailAddress
        {
            Address = "pavelb@contoso.onmicrosoft.com",
            Name = "Pavel Bansky",
            Type = EmailType.Personal
        },
        new TypedEmailAddress
        {
            Address = "pavelb@fabrikam.onmicrosoft.com",
            Name = "Pavel Bansky",
            Type = EmailType.Other,
            OtherLabel = "Volunteer work"
        }
    },
    Phones = new List<Phone>()
    {
        new Phone
        {
            Number = "+1 732 555 0102",
            Type = PhoneType.Business
        }
    }
};

await graphClient.Me.Contacts
    .Request()
    .AddAsync(contact);

```