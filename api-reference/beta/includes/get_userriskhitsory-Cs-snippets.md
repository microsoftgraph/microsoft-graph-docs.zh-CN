---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 31a5aad70a095546c8ae12f17ec00503da8e2325
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34445208"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var history = await graphClient.RiskyUsers["41a31b00-3b3b-42d9-8f1c-6d4f14e74c69"].History
    .Request()
    .GetAsync();

```