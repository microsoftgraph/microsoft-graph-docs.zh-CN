---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b101250d50b1838a2632fb212aaee26a5344f2e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784750"
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

await graphClient.Sites["{site-id}"].Lists["{list-id}"].Items["{listItem-id}"].Fields
    .Request()
    .UpdateAsync(fieldValueSet);

```