---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 6e9dc0d103a417eddaa975f980568ff07fb37323
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34447619"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var plannerTask = await graphClient.Planner.Tasks["01gzSlKkIUSUl6DF_EilrmQAKDhh"]
    .Request()
    .GetAsync();

```