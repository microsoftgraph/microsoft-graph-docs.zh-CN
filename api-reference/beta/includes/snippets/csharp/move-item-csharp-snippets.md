---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2c1cf0ff945b7cb8050572077fe78716ad18e514
ms.sourcegitcommit: af4b2fc18449c33979cf6d75bd680f40602ba708
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/20/2020
ms.locfileid: "48603488"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    ParentReference = new ItemReference
    {
        Id = "new-parent-folder-id"
    },
    Name = "new-item-name.txt"
};

await graphClient.Me.Drive.Items["{item-id}"]
    .Request()
    .UpdateAsync(driveItem);

```