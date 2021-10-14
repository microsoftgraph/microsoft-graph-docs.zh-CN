---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6a2af7c437f3de967ea034c8acf796600921e706018014feb09763a7fbd5556
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218923"
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