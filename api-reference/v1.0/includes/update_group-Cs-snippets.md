---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ea88dd497bff512531bfdf9fb5d635e520fabd08
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34468341"
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