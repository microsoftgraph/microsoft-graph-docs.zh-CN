---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 65ff741223477d0d0f52795779cf68e568f3467a7dcf697679132587a063d721
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57277765"
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