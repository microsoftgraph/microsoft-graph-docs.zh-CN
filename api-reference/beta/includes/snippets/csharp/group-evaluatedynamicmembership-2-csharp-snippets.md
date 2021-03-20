---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1a51348339b2037b1e9116bb6da110ea36dc088
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961863"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var memberId = "319b41e8-d9e4-42f8-bdc9-741113f48b33";

var membershipRule = "(user.displayName -startsWith \"EndTestUser\")";

await graphClient.Groups
    .EvaluateDynamicMembership(memberId,membershipRule)
    .Request()
    .PostAsync();

```