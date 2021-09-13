---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b0f082db8470fa01e11e0760b7ffeed0c4ada6ea47227bb4f5d8d3d3fbd7645
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409705"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var list = new List
{
    DisplayName = "Books",
    Columns = new ListColumnsCollectionPage()
    {
        new ColumnDefinition
        {
            Name = "Author",
            Text = new TextColumn
            {
            }
        },
        new ColumnDefinition
        {
            Name = "PageCount",
            Number = new NumberColumn
            {
            }
        }
    },
    ListInfo = new ListInfo
    {
        Template = "genericList"
    }
};

await graphClient.Sites["{site-id}"].Lists
    .Request()
    .AddAsync(list);

```