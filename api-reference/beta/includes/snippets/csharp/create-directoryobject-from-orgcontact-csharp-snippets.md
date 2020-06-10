---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a8ad3c16acec90a1131b533526c5e0714e09518d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44680667"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var directoryObject = new DirectoryObject
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"directoryObject", "{}"}
    }
};

await graphClient.Contacts["{id}"].MemberOf
    .Request()
    .AddAsync(directoryObject);

```