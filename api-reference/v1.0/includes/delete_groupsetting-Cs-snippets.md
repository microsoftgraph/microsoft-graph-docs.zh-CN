---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ac7a5220305ade46784fe47cf9ca27499b8a93b1
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34458829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.GroupSettings["{id}"]
    .Request()
    .DeleteAsync();

```