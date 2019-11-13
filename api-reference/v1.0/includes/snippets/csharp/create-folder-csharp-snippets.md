---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3c1e2bca2fe9b76d26cb1eee22ac545f8fbd5d8d
ms.sourcegitcommit: fa08172601324fc01b090f8135fba4600bd1a9f8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/13/2019
ms.locfileid: "38302637"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "New Folder",
    Folder = new Folder
    {
    },
    AdditionalData = new Dictionary<string, object>()
    {
        {"@microsoft.graph.conflictBehavior","rename"}
    }
};

await graphClient.Me.Drive.Root.Children
    .Request()
    .AddAsync(driveItem);

```