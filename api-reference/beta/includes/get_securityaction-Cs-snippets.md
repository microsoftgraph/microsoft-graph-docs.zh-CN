---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 0e1382105615d0a82dddc60e590949e21a3036e6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446321"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var securityAction = await graphClient.Security.SecurityActions["{id}"]
    .Request()
    .GetAsync();

```