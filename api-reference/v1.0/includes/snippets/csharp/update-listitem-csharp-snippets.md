---
description: 自动生成的文件。 不修改
ms.openlocfilehash: fe232c0c5a555fde0f22c103ef110166fcb110d6
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35467355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fieldValueSet = new FieldValueSet
{
    Color = "Fuchsia",
    Quantity = 934
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Fields
    .Request()
    .UpdateAsync(fieldValueSet);

```