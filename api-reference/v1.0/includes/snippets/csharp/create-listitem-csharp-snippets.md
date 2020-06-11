---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d93bef0bf2e3a4396f11a5ec3512bf9bc078806c
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44684838"
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