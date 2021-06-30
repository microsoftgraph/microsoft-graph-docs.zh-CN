---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 75d73e2fb3c95f054118bb2e8299d9d0e6c485dd
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208287"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

var availability = "Available";

var activity = "Available";

var expirationDuration = new Duration("PT1H");

await graphClient.Users["{user-id}"].Presence
    .SetPresence(sessionId,availability,activity,expirationDuration)
    .Request()
    .PostAsync();

```