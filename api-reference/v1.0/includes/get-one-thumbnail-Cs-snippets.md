---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8a2135be2fa313fd8cee336096932609a25f7c53
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462729"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var {size} = await graphClient.Me.Drive.Items["{item-id}"].Thumbnails["{thumb-id}"].{size}
    .Request()
    .GetAsync();

```