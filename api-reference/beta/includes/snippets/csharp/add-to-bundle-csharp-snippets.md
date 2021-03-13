---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d419c6cfc6796a05cafe843721d2b7b4a9d66aa5
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50774395"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = new DriveItem
{
    Id = "123456!87"
};

await graphClient.Drive.Bundles["{driveItem-id}"].Children
    .Request()
    .AddAsync(driveItem);

```