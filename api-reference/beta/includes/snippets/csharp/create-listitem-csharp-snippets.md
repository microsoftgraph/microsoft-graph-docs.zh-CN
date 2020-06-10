---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 84e4582a7a728680a848bbe80dd013bd4efe8266
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var fieldValueSet = new FieldValueSet
{
    AdditionalData = new Dictionary<string, object>()
    {
        {"Color", "Fuchsia"},
        {"Quantity", "934"}
    }
};

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{item-id}"].Fields
    .Request()
    .UpdateAsync(fieldValueSet);

```