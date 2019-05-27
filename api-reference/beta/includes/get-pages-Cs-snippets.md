---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 40d3e5d6737cf7f674612423222f0e7091047970
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34435996"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var pages = await graphClient.Sites["{site-id}"].Pages
    .Request()
    .GetAsync();

```