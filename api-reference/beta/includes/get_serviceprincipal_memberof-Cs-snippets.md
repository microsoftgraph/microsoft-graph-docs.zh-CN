---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a891fbc5807ebc35d07056057f7b62eda7ced0fe
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446181"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberOf = await graphClient.ServicePrincipals["{id}"].MemberOf
    .Request()
    .GetAsync();

```