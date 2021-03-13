---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f17580290f970818f81b8d044543aa48c9e09e1
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50780269"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Shared legal agreements"
};

await graphClient.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```