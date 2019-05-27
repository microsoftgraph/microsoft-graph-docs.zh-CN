---
description: 自动生成的文件。 不修改
ms.openlocfilehash: a0cce39cc24a98e3c0a19968d1d8f0b40292a6c6
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34472411"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var createdObjects = await graphClient.Me.CreatedObjects
    .Request()
    .GetAsync();

```