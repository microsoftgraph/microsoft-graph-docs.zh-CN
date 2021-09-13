---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 88d6eece9608673f32bd162784c746365a07b146
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59130116"
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

await graphClient.Sites["{site-id}"].TermStore.Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .UpdateAsync(term);

```