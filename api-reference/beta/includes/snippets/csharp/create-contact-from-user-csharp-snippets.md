---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f0f35fe4cbd8a4b432e0fe4d59f3e887d59a094f0c54f6ed3ead36c76c3ff806
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104662"
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