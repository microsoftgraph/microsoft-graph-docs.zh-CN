---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a19314d30cc280691108a08da9c79155916ef81
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786162"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeOffRequests["{timeOffRequest-id}"]
    .Request()
    .DeleteAsync();

```