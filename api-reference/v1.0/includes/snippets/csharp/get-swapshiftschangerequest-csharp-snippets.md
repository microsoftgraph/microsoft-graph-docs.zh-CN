---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 613bdc3338007896a6fbbdbc89c0ef25b25d1d5f
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequest = await graphClient.Teams["{teamId}"].Schedule.SwapShiftsChangeRequests["{swapShiftsChangeRequestId}"]
    .Request()
    .GetAsync();

```