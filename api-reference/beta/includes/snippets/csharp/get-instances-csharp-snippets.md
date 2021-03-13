---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b715fed08892659087f7daa4076e6065a00545f0
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50784032"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var queryOptions = new List<QueryOption>()
{
    new QueryOption("startDateTime", "2019-04-08T09:00:00.0000000"),
    new QueryOption("endDateTime", "2019-04-30T09:00:00.0000000")
};

var instances = await graphClient.Me.Events["{event-id}"].Instances
    .Request( queryOptions )
    .Select("subject,bodyPreview,seriesMasterId,type,recurrence,start,end")
    .GetAsync();

```