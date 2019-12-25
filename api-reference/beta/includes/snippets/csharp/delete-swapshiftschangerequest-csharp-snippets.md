---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 930d151acc5cdadd4a63030bfea9bf268c1163d4
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870849"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

await graphClient.Teams["{id}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .DeleteAsync();

```