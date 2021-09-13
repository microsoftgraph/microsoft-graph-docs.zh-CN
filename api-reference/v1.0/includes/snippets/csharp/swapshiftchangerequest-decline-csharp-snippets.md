---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf50f3b3754bdc0d00204ba7e68bf067f97e4f0c278875783527980daac02733
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57161986"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.SwapShiftsChangeRequests["{swapShiftsChangeRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```