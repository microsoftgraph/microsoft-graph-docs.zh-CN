---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31d28474e92ddf1d0341c6c256fe530b4b7914baf196fccbc81e5a2a89e2af65
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56903159"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    AllowedToUseSSPR = true
};

await graphClient.Policies.AuthorizationPolicy["{authorizationPolicy-id}"]
    .Request()
    .UpdateAsync(authorizationPolicy);

```