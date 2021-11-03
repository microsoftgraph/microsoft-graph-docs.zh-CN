---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cacaa28b48aedfd740e34cd5b0b6cbea9e299758
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60718092"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var term = new Microsoft.Graph.TermStore.Term
{
    Labels = new List<Microsoft.Graph.TermStore.LocalizedLabel>()
    {
        new Microsoft.Graph.TermStore.LocalizedLabel
        {
            LanguageTag = "en-US",
            Name = "Car",
            IsDefault = true
        }
    }
};

await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Children
    .Request()
    .AddAsync(term);

```