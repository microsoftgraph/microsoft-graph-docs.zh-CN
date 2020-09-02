---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 62d974d80525411c47bbbd2cbec56849317d5a9f
ms.sourcegitcommit: 726f20403323be7d267b67c2764ed7c244e02ee1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/02/2020
ms.locfileid: "47330136"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Term
{
    Labels = new List<LocalizedLabel>()
    {
        new LocalizedLabel
        {
            LanguageTag = "en-US",
            Name = "Car",
            IsDefault = true
        }
    }
};

await graphClient.TermStore.Sets["{setId}"].Terms
    .Request()
    .AddAsync(term);

```