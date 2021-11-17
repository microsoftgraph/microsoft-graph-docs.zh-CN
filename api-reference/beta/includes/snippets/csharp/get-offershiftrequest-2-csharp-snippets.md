---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1ac143aa31adc49310f3f84de1ece251f013a3df518c2ba44c2d440b32169e81
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57215827"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequests = await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests
    .Request()
    .GetAsync();

```