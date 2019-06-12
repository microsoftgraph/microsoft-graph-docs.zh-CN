---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 711e0ffeabd73b0ce6c8873fc4da7bd394f7bb39
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34843484"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var user = await graphClient.Users["{user-id}"]
    .Request()
    .GetAsync();

```