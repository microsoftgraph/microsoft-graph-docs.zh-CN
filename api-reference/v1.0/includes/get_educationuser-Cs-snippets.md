---
description: 自动生成的文件。 不修改
ms.openlocfilehash: ebe7989c3ff5d85546aca4413499854b072c26ac
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34479544"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var educationUser = await graphClient.Education.Users["{user-id}"]
    .Request()
    .GetAsync();

```