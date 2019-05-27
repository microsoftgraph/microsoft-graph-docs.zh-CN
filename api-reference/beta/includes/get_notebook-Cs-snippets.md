---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 672ec71879101810db62196e93b61fa83f4e1d77
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34448389"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var notebook = await graphClient.Me.Onenote.Notebooks["{id}"]
    .Request()
    .GetAsync();

```