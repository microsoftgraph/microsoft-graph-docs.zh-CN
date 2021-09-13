---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9547f4aa71e654ee4a084d18e69c6600addf742e99337e451a347501f892acc
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57332164"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authorizationPolicy = new AuthorizationPolicy
{
    AllowedToUseSSPR = true
};

await graphClient.Policies.AuthorizationPolicy
    .Request()
    .UpdateAsync(authorizationPolicy);

```