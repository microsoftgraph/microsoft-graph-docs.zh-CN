---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c52999d92ffd7048080e0381185e3a63aec49e2d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48606497"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Self help community for golf",
    DisplayName = "Golf Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "golfassist",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```