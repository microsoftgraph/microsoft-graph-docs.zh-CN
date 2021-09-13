---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 212f6b11d2692d4192f0fda7ec47366409864395673cdab6a73d286a791b9f73
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332750"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Sorry, you can't offer this shift.";

await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests["{offerShiftRequest-id}"]
    .Decline(message)
    .Request()
    .PostAsync();

```