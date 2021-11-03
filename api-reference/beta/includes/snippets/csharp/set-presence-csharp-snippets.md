---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b3d814945a9348a3fae0e3e11ce9cbd4ec3eaf41
ms.sourcegitcommit: c7ff992ef63e480d070421ba99b28ee129cb6acb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/03/2021
ms.locfileid: "60697001"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

var availability = "Available";

var activity = "Available";

var expirationDuration = new Duration("PT1H");

await graphClient.Users["{user-id}"].Presence
    .SetPresence(availability,activity,sessionId,expirationDuration)
    .Request()
    .PostAsync();

```