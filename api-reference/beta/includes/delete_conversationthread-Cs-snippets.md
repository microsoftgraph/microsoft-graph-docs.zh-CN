---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 070506d6496492be405a4e7691c0fcf4bbebb908
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34438719"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"].Threads["{id}"]
    .Request()
    .DeleteAsync();

```