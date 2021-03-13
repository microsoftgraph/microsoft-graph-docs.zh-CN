---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7592ff5f6b5d7d462287a673457e3f38767895bb
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50776093"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var openShiftChangeRequest = await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Request()
    .GetAsync();

```