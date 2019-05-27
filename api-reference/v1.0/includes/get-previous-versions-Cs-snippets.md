---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 5899a66e621e2053b71f970de184b67ea5917c95
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34462652"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var versions = await graphClient.Me.Drive.Items["{item-id}"].Versions
    .Request()
    .GetAsync();

```