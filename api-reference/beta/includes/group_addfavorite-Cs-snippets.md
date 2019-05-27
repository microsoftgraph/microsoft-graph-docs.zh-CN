---
description: 自动生成的文件。 不修改
ms.openlocfilehash: f953d9ad67ca4558856cef72c7b961b5c9fe027d
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34444893"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Groups["{id}"]
    .AddFavorite()
    .Request()
    .PostAsync();

```