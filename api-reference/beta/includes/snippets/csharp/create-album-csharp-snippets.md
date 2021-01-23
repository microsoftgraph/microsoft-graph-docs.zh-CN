---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3084bbd1bcbd61d373296c01cd0566a6b7954d5a
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49945231"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "My Day at the Beach",
    Bundle = new Bundle
    {
        Album = new Album
        {
        }
    },
    Children = new DriveItemChildrenCollectionPage()
    {
        new DriveItem
        {
            Id = "1234asdf"
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