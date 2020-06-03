---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 547fd503603a8d7b3d06cf27ba81df07ba3dcfa4
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44217631"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var message = "Sorry, you can't offer this shift.";

await graphClient.Teams["{teamId}"].Schedule.OfferShiftRequests["{offerShiftRequestId}"]
    .Decline(message)
    .Request()
    .PostAsync();

```