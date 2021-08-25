---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 70083f97879b8cf1d2edd23c44fc4cc6f423dce9
ms.sourcegitcommit: 9b8abc940a68dac6ee5da105ca29800cb59775f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/25/2021
ms.locfileid: "58514219"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var sessionId = "22553876-f5ab-4529-bffb-cfe50aa89f87";

await graphClient.Users["{user-id}"].Presence
    .ClearPresence(sessionId)
    .Request()
    .PostAsync();

```