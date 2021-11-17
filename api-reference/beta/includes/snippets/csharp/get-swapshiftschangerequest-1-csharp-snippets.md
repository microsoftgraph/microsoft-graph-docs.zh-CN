---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00ddb38cea8f61c2ef6cae60d3802bad9f55d2e872f37f25d10f7b65236bab2d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57103828"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var swapShiftsChangeRequest = await graphClient.Teams["{team-id}"].Schedule.SwapShiftsChangeRequests["{swapShiftsChangeRequest-id}"]
    .Request()
    .GetAsync();

```