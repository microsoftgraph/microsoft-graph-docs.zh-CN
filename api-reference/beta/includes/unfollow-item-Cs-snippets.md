---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 3b8a4c2fe8c6efd3231eeb06998b44e303c6d7e8
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462041"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Me.Drive.Following["{item-id}"]
    .Request()
    .DeleteAsync();

```