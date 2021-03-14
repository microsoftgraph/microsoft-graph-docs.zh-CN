---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfd9a83ed7b6f2cdcfd9f41e4a5224c26093f052
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50778653"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```