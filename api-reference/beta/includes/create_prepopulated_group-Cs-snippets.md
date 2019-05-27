---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b4c0145ef94b4c22d9c34aaa90bb923e43270e40
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34439951"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Group with designated owner and members",
    DisplayName = "Operations group",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "operations2019",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```