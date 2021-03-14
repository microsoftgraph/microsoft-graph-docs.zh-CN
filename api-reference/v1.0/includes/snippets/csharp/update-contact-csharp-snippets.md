---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b71136330b1e5c9dd1aa64023c3c295dd04db86
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50788002"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var contact = new Contact
{
    HomeAddress = new PhysicalAddress
    {
        Street = "123 Some street",
        City = "Seattle",
        State = "WA",
        PostalCode = "98121"
    },
    Birthday = DateTimeOffset.Parse("1974-07-22")
};

await graphClient.Me.Contacts["{contact-id}"]
    .Request()
    .UpdateAsync(contact);

```