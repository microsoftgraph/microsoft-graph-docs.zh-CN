---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 32fc4220f0518c3708a92ae233f1879cb58c2468
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34466307"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var onenoteSection = await graphClient.Me.Onenote.Sections["{id}"]
    .Request()
    .GetAsync();

```