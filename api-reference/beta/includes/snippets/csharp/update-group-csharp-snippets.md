---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea88dd497bff512531bfdf9fb5d635e520fabd08
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35711716"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var group = new Group
{
    Description = "description-value",
    DisplayName = "displayName-value",
    GroupTypes = new List<String>()
    {
        "groupTypes-value"
    },
    Mail = "mail-value",
    MailEnabled = true,
    MailNickname = "mailNickname-value"
};

await graphClient.Groups["{id}"]
    .Request()
    .UpdateAsync(group);

```