---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 3bfdf38efc08e91917cf09dbc8ce93e3c2738c04
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59777159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Channels["{channel-id}"]
    .RemoveEmail()
    .Request()
    .PostAsync();

```