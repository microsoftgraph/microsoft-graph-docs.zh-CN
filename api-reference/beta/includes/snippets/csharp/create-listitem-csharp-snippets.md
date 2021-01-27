---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d93bef0bf2e3a4396f11a5ec3512bf9bc078806c
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015474"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var listItem = new ListItem
{
    Fields = new FieldValueSet
    {
        AdditionalData = new Dictionary<string, object>()
        {
            {"Title", "Widget"},
            {"Color", "Purple"},
            {"Weight", "32"}
        }
    }
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items
    .Request()
    .AddAsync(listItem);

```