---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d28ed4a9b659ee6675de1490dfd0eeca9cc02ebc
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48620978"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var value = new List<TiIndicator>()
{
    new TiIndicator
    {
        Id = "c6fb948b-89c5-3bba-a2cd-a9d9a1e430e4",
        AdditionalInformation = "mytest"
    },
    new TiIndicator
    {
        Id = "e58c072b-c9bb-a5c4-34ce-eb69af44fb1e",
        AdditionalInformation = "test again"
    }
};

await graphClient.Security.TiIndicators
    .UpdateTiIndicators(value)
    .Request()
    .PostAsync();

```