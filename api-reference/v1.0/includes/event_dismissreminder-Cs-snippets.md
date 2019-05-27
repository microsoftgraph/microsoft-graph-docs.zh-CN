---
description: 自动生成的文件。 不修改
ms.openlocfilehash: b27a9f0711759f53e42f7501a4f95c32128fb4eb
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34457794"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Events["{id}"]
    .DismissReminder()
    .Request()
    .PostAsync();

```