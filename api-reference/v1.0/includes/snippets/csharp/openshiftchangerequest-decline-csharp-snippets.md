---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9b066007c5883625c0740e7c9bad1b56efa70025297bf08ab9de979493fefb59
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57218725"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "message-value";

await graphClient.Teams["{team-id}"].Schedule.OpenShiftChangeRequests["{openShiftChangeRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```