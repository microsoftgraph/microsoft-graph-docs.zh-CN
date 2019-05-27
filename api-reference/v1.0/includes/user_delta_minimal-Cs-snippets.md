---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3235e68f041adbf09c3b3c2b082b60138a2bf384
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34434264"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Users.Delta()
    .Request()
    .Header("Prefer","return=minimal")
    .Select( e => new {
             e.DisplayName,
             e.JobTitle,
             e.MobilePhone 
             })
    .GetAsync();

```