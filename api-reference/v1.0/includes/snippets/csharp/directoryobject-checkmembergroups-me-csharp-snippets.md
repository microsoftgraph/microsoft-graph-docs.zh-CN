---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df9788352beafb7595f7faa9f7f74e9a0f087b01
ms.sourcegitcommit: e497ed9bb56400bdd2bb53d52ddf057d9966220b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/30/2021
ms.locfileid: "61224029"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var groupIds = new List<String>()
{
    "fee2c45b-915a-4a64b130f4eb9e75525e",
    "4fe90ae065a-478b9400e0a0e1cbd540"
};

await graphClient.Me
    .CheckMemberGroups(groupIds)
    .Request()
    .PostAsync();

```