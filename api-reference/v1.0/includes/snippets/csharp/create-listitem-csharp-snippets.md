---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 347b4f4806a31bd7d4c1a4d63d615d755d9741779dfdd45db526f80eda3bd944
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162574"
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