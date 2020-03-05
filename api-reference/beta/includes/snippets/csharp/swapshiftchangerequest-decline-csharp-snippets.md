---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 095cf84ead44972ff0ca8fa5f3b316bf6c43d27e
ms.sourcegitcommit: d419565add1f731be50c9b5911eb1310fa007097
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2020
ms.locfileid: "42280648"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{id}"].Schedule.SwapShiftsChangeRequests["{swapShiftChangeRequestId}"]
    .Decline(message)
    .Request()
    .PostAsync();

```