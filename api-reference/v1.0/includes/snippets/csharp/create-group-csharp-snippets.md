---
description: 自动生成的文件。 不修改
ms.openlocfilehash: be9c99e5b77edda415f3bdf19561caf9e152e377
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467523"
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