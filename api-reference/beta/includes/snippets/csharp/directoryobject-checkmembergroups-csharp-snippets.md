---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 952496e812d2ecc3dfa41942a27819188af6ce34
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35706886"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "fee2c45b-915a-4a64-b130-f4eb9e75525e",
    "4fe90ae7-065a-478b-9400-e0a0e1cbd540"
};

await graphClient.Me
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```