---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71afc8b10c0d3193cd3b0fb81c05489c67ec43c9a0338b5599ab4f33f75e7df7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902470"
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

await graphClient.TermStore.Sets["{termStore.set-id}"].Terms["{termStore.term-id}"]
    .Request()
    .UpdateAsync(term);

```