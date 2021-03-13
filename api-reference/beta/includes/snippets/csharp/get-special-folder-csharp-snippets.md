---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44486124a6a20dc7e3dbead689611ce50e7b5b39
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50787262"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var driveItem = await graphClient.Me.Drive.Special["{driveItem-id}"]
    .Request()
    .GetAsync();

```