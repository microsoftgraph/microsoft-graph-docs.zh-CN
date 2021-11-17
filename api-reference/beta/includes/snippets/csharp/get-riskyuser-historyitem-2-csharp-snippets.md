---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2a1050c2d8e26525ddfcd01f3727ee1d79782c6e8b9ce19e004fb09ddb73327b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903085"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var riskyUserHistoryItem = await graphClient.IdentityProtection.RiskyUsers["{riskyUser-id}"].History["{riskyUserHistoryItem-id}"]
    .Request()
    .GetAsync();

```