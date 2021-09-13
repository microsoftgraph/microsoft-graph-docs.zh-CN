---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8295c38c9e8d9fc7f35a9a4ca0a470e247e04786c99cb7df53689adb1e469e83
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409089"
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
        {"@microsoft.graph.conflictBehavior", "rename"}
    }
};

await graphClient.Me.Drive.Root.Children
    .Request()
    .AddAsync(driveItem);

```