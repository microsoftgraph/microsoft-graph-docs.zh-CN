---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 47f2b50071233c6716aee67ccd246e8f022adab4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446807"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUser = await graphClient.RiskyUsers["c2b6c2b9-dddc-acd0-2b39-d519d803dbc3"]
    .Request()
    .GetAsync();

```