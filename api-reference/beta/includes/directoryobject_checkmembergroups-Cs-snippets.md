---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 952496e812d2ecc3dfa41942a27819188af6ce34
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34437263"
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