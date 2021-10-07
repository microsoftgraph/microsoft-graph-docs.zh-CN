---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d877fbc4fbb9bd7ff0b3cdb382ffa688005da4cb0750bdecfa7313616b6415b
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104373"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new PasswordlessMicrosoftAuthenticatorAuthenticationMethodConfiguration
{
    State = AuthenticationMethodState.Enabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```