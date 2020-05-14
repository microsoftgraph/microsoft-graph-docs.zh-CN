---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00bfbf540dae9d7015c894cd093e642b9ba769f4
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2020
ms.locfileid: "44217923"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{teamId}"].Schedule.TimeOffRequests["{timeOffRequestId}"]
    .Approve(message)
    .Request()
    .PostAsync();

```