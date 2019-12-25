---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5b77175d2920be410abebe94a2f46ac9603ff6a6
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870788"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequests = new SwapShiftsChangeRequest
{
    RecipientShiftId = "recipientShiftId-value"
};

await graphClient.Teams["{id}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .UpdateAsync(swapShiftsChangeRequests);

```