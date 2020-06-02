---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e4af07aa548115ea66030bd413030df4d2d45fed
ms.sourcegitcommit: 94c8985a3956622ea90f7e641f894d57b0982eb9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/02/2020
ms.locfileid: "44219221"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{teamId}"].Schedule.TimeOffRequests["{timeOffRequestId}"]
    .Request()
    .DeleteAsync();

```