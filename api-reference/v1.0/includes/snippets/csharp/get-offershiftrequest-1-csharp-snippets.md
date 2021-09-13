---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 292d89facb1472d04409465b0c85db7fd6204def7e56e9823d5176a326328058
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105355"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequest = await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests["{offerShiftRequest-id}"]
    .Request()
    .GetAsync();

```