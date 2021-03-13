---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6f1922a2fcae1cc752fd370e1c94f9f726ce2b76
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50808331"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{team-id}"].Schedule.TimeOffReasons["{timeOffReason-id}"]
    .Request()
    .DeleteAsync();

```