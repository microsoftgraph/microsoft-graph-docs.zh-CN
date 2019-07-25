---
description: 自动生成的文件。 不修改
ms.openlocfilehash: cd70bdb94027d811395ee4877f513f55d6cd09d0
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35723336"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    GivenName = "Pavel",
    Surname = "Bansky",
    EmailAddresses = new List<EmailAddress>()
    {
        new EmailAddress
        {
            Address = "pavelb@fabrikam.onmicrosoft.com",
            Name = "Pavel Bansky"
        }
    },
    BusinessPhones = new List<String>()
    {
        "+1 732 555 0102"
    }
};

await graphClient.Me.Contacts
    .Request()
    .AddAsync(contact);

```