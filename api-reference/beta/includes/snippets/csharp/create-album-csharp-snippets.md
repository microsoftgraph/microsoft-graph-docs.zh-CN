---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31982cb502ac21808d32048bebf5fc724a9501d9
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302622"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "My Day at the Beach",
    AdditionalData = new Dictionary<string, object>()
    {
        {"@name.conflictBehavior","rename"}
    },
    Bundle = new Bundle
    {
        Album = new Album
        {
        }
    },
    Children = new List<DriveItem>()
    {
        new DriveItem
        {
            Id = "1234asdf"
        }
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```