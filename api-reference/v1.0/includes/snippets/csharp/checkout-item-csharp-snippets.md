---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 42b79ae2a39c87b502a9072fa0b19d34698f6383
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50779096"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Drives["{drive-id}"].Items["{driveItem-id}"]
    .Checkout()
    .Request()
    .PostAsync();

```