---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb40481bc78bbe26a41a349760e454cfb677de9b
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280659"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{id}"].Schedule.SwapShiftsChangeRequests["{swapShiftChangeRequestId}"]
    .Approve(message)
    .Request()
    .PostAsync();

```