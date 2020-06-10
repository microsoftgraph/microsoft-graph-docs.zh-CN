---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc8259d4f30f1075e640609b1cfbcf6eafd34843
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681073"
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

await graphClient.Devices["{id}"].RegisteredUsers.References
    .Request()
    .AddAsync(directoryObject);

```