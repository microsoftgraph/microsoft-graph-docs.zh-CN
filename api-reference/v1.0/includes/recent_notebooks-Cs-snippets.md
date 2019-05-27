---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 68490dbb5aa9c5617abd8b36f05db8c580e2c9c7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34450629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var getRecentNotebooks = await graphClient.Me.Onenote.Notebooks.GetRecentNotebooks(true)
    .Request()
    .GetAsync();

```