---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 369396d02b2335a19438be2e9565b44950744ae3
ms.sourcegitcommit: d8a425766aa6a56027b8576bbec6a9d1ae3e079c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2019
ms.locfileid: "36845963"
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

await graphClient.Me.Contacts["{id}"]
    .Request()
    .UpdateAsync(contact);

```