---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cfb2e25b8f08dcb910cfbd49a4bf5b64953cc917
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945285"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var offerShiftRequests = await graphClient.Teams["{team-id}"].Schedule.OfferShiftRequests
    .Request()
    .GetAsync();

```