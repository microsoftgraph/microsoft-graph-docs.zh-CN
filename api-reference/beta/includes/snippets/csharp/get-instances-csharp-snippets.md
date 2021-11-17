---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87dc74e624c45db27f1c750a7b1891fee08a36cdfff266f5d0ea8284a64e116c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162903"
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