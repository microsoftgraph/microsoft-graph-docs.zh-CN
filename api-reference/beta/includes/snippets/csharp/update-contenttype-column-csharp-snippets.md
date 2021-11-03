---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8749496574fc3494330fa4e74165cb852c9f15d36138ed4ddc42d33c8b691360
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278345"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var columnDefinition = new ColumnDefinition
{
    Required = true,
    Hidden = false,
    PropagateChanges = false
};

await graphClient.Sites["{site-id}"].ContentTypes["{contentType-id}"].Columns["{columnDefinition-id}"]
    .Request()
    .UpdateAsync(columnDefinition);

```