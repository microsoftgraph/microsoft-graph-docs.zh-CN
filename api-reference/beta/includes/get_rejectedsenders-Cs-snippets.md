---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 22e9e161db499230e238f2a8b8bc325922b1e0ab
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34446842"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var rejectedSenders = await graphClient.Groups["{id}"].RejectedSenders
    .Request()
    .GetAsync();

```