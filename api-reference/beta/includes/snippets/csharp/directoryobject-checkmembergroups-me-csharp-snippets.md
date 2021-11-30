---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 952496e812d2ecc3dfa41942a27819188af6ce34
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61225009"
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