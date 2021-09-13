---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1bd9d855d193e95c86e43449080eb71c3c24f2cf5a98879c87c666486d3ecfdd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104328"
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