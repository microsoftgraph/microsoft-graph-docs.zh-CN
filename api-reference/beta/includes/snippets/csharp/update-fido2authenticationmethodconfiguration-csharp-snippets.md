---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d24cb9901ddea53a6d40567819aa2f03b9ce6e5b09ca6d7aa2718b797648b184
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163427"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new Fido2AuthenticationMethodConfiguration
{
    State = AuthenticationMethodState.Enabled,
    IsAttestationEnforced = true
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```