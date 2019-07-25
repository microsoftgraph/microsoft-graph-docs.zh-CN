---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 040fc1bdb7a0a5519d7790e93f84efc000c72bb7
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35705942"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var comment = "Updating the latest guidelines";

await graphClient.Drives["{drive-id}"].Items["{item-id}"]
    .Checkin(checkInAs,comment)
    .Request()
    .PostAsync();

```