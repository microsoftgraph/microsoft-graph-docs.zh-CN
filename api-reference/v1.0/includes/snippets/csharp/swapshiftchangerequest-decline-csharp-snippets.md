---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: dec4c4bc96b809bee9fade1683a2be774fb95306
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50801980"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.SwapShiftsChangeRequests["{swapShiftsChangeRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```