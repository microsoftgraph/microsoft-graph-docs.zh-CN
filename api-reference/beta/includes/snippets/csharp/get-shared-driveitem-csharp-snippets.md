---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 556fcc50d6f792f8ec31260481ac96add40aa113
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779941"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Shares["{sharedDriveItem-id}"].DriveItem
    .Request()
    .GetAsync();

```