---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ec5f046a9dbe7cc61f49c2bddad962c57106f20d
ms.sourcegitcommit: be796d6a7ae62f052c381d20207545f057b184d9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/14/2020
ms.locfileid: "48462642"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Microsoft.Graph.TermStore.Term
{
    Labels = new List<Microsoft.Graph.TermStore.LocalizedLabel>()
    {
        new Microsoft.Graph.TermStore.LocalizedLabel
        {
            Name = "changedLabel",
            LanguageTag = "en-US",
            IsDefault = true
        }
    }
};

await graphClient.TermStore.Sets["{setId}"].Terms["{termId}"]
    .Request()
    .UpdateAsync(term);

```