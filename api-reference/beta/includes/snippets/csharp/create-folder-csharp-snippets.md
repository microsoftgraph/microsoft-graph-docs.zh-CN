---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 4d98b01bceb2afa08c9f6c84ae8f531c0d4f104d
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35712829"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "New Folder",
    Folder = new Folder
    {
    },
    @microsoft.graph.conflictBehavior = "rename"
};

await graphClient.Me.Drive.Root.Children
    .Request()
    .AddAsync(driveItem);

```