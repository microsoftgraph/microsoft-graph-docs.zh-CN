---
description: 自动生成的文件。 不修改
ms.openlocfilehash: 8d2653638dc9afc3f2f80d1eaaac5f357d0f16a2
ms.sourcegitcommit: 4fa6b745383bb0c1864b65d612d811d64cdc079f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/25/2019
ms.locfileid: "34460915"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var parentReference = new ItemReference
{
    DriveId = "6F7D00BF-FC4D-4E62-9769-6AEA81F3A21B",
    Id = "DCD0D3AD-8989-4F23-A5A2-2C086050513F"
};

var name = "contoso plan (copy).txt";

await graphClient.Me.Drive.Items["{item-id}"]
    .Copy(name,parentReference)
    .Request()
    .PostAsync();

```