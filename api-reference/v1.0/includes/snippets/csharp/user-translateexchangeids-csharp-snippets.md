---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 345c58fc0dc9263f0c91efbdc14dcc978451b75d
ms.sourcegitcommit: 997fbfe36b518e0a8c230ae2e62666bb5c829e7e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/19/2019
ms.locfileid: "37041902"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var inputIds = new List<String>()
{
    "{rest-formatted-id-1}",
    "{rest-formatted-id-2}"
};

var sourceIdType = ExchangeIdFormat.RestId;

var targetIdType = ExchangeIdFormat.RestImmutableEntryId;

await graphClient.Me
    .TranslateExchangeIds(inputIds,targetIdType,sourceIdType)
    .Request()
    .PostAsync();

```