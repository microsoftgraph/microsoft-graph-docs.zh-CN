---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 345c58fc0dc9263f0c91efbdc14dcc978451b75d
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48622291"
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