---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aa561925cbe361b8993a77a03393d9a75717622
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780745"
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

await graphClient.Contacts["{orgContact-id}"].MemberOf
    .Request()
    .AddAsync(directoryObject);

```