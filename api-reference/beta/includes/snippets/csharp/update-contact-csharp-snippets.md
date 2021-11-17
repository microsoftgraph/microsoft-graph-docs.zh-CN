---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0caf3740a397b20e3f8b6c2ae9c9dee8e160d18a73f41acb42539e07f626f374
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57274414"
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