---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d445039ee440477a8b0c68dcf368973d17182030
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219210"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{teamId}"].Schedule.SwapShiftsChangeRequests["{swapShiftChangeRequestId}"]
    .Approve(message)
    .Request()
    .PostAsync();

```