---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 857aef821e1b51555011cf3409468a75d27adaed
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34454879"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var delta = await graphClient.Me.Drive.Root.Delta('1230919asd190410jlka')
    .Request()
    .GetAsync();

```