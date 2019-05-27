---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 360ebe3b06dcd09e484bff21fe3637cf7772d6ad
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444480"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var activities = await graphClient.Me.Drive.Activities
    .Request()
    .GetAsync();

```