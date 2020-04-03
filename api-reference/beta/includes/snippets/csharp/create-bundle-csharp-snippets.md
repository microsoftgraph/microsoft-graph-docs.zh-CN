---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a87355ac5e1431d24d87a60826694f4032bf9ab
ms.sourcegitcommit: bd40e302ce04b686e86989246ab7c4cc9ad3f320
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2020
ms.locfileid: "43127106"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Just some files",
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.conflictBehavior","rename"}
    },
    Bundle = new Bundle
    {
    },
    Children = new List<DriveItem>()
    {
        new DriveItem
        {
            Id = "1234asdf"
        },
        new DriveItem
        {
            Id = "1234qwerty"
        }
    }
};

await graphClient.Drive.Bundles
    .Request()
    .AddAsync(driveItem);

```