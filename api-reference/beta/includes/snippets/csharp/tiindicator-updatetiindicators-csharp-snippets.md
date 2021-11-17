---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 89fbf086740f0c83ec40591277fd662fb414a550dc4a3c0dd9d96fc5713a238e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57220186"
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