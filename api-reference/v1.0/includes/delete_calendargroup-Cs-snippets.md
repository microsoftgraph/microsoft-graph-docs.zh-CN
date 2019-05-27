---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3a3f953697a333f17e730a818d6b892a93872171
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34459633"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.CalendarGroups["{id}"]
    .Request()
    .DeleteAsync();

```