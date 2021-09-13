---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4b20dd5eb52cda46f1415ac1540eccd45740c42717da94fc8b461fa7d666174b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162945"
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