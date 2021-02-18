---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 999af81d8149264503d8602a394224e51887dd1b
ms.sourcegitcommit: 42fdb068616222eb6b0813e93b33e830fc7eedc0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/17/2021
ms.locfileid: "50274837"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var timeOffRequest = await graphClient.Teams["{teamId}"].Schedule.TimeOffRequests["{timeOffRequestId}"]
    .Request()
    .GetAsync();

```