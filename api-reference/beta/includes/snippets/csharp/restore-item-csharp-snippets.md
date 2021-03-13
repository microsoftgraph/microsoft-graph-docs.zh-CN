---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba5afc305d5637d77af1a603d25aa381ad4fb968
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50791550"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    Id = "String"
};

var name = "String";

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Restore(parentReference,name)
    .Request()
    .PostAsync();

```