---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 18c1f62369bceb174db1435d3fe454448f037a9f24f6504f2a3a2d6bb1566ee7
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332629"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    ParentReference = new ItemReference
    {
        Id = "{new-parent-folder-id}"
    },
    Name = "new-item-name.txt"
};

await graphClient.Me.Drive.Items["{driveItem-id}"]
    .Request()
    .UpdateAsync(driveItem);

```