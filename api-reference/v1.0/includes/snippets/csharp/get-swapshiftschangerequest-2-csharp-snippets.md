---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7d18ba151d05ad76e1be6496e08687ddd7f40dd9f9542ca5b657b98a784011ee
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57333468"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequests = await graphClient.Teams["{team-id}"].Schedule.SwapShiftsChangeRequests
    .Request()
    .GetAsync();

```