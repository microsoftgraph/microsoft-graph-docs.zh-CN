---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3d64924185fc5aec26684203b6f92cdec4289c964c5278ce567decc4315f8b3e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105010"
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