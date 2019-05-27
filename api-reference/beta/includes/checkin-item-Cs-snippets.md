---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 040fc1bdb7a0a5519d7790e93f84efc000c72bb7
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34451873"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Updating the latest guidelines";

await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .Checkin(checkInAs,comment)
    .Request()
    .PostAsync();

```