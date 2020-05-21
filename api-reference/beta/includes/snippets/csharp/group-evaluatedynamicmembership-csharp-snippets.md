---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d1a51348339b2037b1e9116bb6da110ea36dc088
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333022"
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