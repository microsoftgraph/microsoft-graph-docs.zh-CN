---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8674dcca8596702cb231c68fd9d571f03c770d5b94b960b6f15d4123b4ffde4e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105172"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Name = "Just some files",
    Bundle = new Bundle
    {
    },
    Children = new DriveItemChildrenCollectionPage()
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