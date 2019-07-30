---
description: 自动生成的文件。 不修改
ms.openlocfilehash: c9b19516ac5ea77212a36d5cd99317666b9bbf92
ms.sourcegitcommit: 56c0b609dfb1bc5d900956f407d107cdab7086e8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/30/2019
ms.locfileid: "35932643"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Id = "123456!87"
};

await graphClient.Drive.Bundles["{bundle-id}"].Children
    .Request()
    .AddAsync(driveItem);

```