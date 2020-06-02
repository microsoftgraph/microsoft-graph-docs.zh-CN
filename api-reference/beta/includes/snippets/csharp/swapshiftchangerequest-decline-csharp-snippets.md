---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2474b3e27a65d1cd36139d4e4301b23b2cd6751c
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219215"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{teamId}"].Schedule.SwapShiftsChangeRequests["{swapShiftChangeRequestId}"]
    .Decline(message)
    .Request()
    .PostAsync();

```