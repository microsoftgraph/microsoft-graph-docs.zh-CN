---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ca53dfaae351f3e574313c7bdc3218229df09b42
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777190"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .ProvisionEmail()
    .Request()
    .PostAsync();

```