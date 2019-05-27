---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 83406446c4cb9345936e14cc4ae4b9b0eea95c1f
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462997"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var instances = await graphClient.Me.Events["AAMkAGUzYRgWAAA="].Instances
    .Request()
    .Select( e => new {
             e.Subject,
             e.BodyPreview,
             e.SeriesMasterId,
             e.Type,
             e.Recurrence,
             e.Start,
             e.End 
             })
    .GetAsync();

```