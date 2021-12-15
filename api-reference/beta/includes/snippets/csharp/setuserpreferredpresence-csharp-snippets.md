---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 836e0e3bc750d60a97dd2cfa7b5559077c5b6aab
ms.sourcegitcommit: c47e3d1f3c5f7e2635b2ad29dfef8fe7c8080bc8
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/15/2021
ms.locfileid: "61526092"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var availability = "DoNotDisturb";

var activity = "DoNotDisturb";

var expirationDuration = new Duration("PT8H");

await graphClient.Users["{user-id}"].Presence
    .SetUserPreferredPresence(availability,activity,expirationDuration)
    .Request()
    .PostAsync();

```