---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 1ff0ac226b099411f11695298f95e7588bd862a4
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34436430"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var AudioRoutingGroup = await graphClient.App.Calls["{id}"].AudioRoutingGroups["{id}"]
    .Request()
    .GetAsync();

```