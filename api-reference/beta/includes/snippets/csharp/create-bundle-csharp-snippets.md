---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f32bbda9b6849ebfbde9aca14b8e6ab4c848b54
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44683715"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Just some files",
    Bundle = new Bundle
    {
    },
    Children = (IDriveItemChildrenCollectionPage)new List<DriveItem>()
    {
        new DriveItem
        {
            Id = "1234asdf"
        },
        new DriveItem
        {
            Id = "1234qwerty"
        }
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.conflictBehavior", "rename"}
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```