---
description: 自动生成的文件。 不修改
ms.openlocfilehash: be9c99e5b77edda415f3bdf19561caf9e152e377
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35722802"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "Self help community for library",
    DisplayName = "Library Assist",
    GroupTypes = new List<String>()
    {
        "Unified"
    },
    MailEnabled = true,
    MailNickname = "library",
    SecurityEnabled = false
};

await graphClient.Groups
    .Request()
    .AddAsync(group);

```