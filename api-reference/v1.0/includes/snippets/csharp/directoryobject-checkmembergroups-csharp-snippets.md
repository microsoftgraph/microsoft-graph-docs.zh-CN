---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 963a06592c2d7792555f9881d7ee7cbaf5a46e42
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791013"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "fee2c45b-915a-4a64b130f4eb9e75525e",
    "4fe90ae065a-478b9400e0a0e1cbd540"
};

await graphClient.DirectoryObjects["{directoryObject-id}"]
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```