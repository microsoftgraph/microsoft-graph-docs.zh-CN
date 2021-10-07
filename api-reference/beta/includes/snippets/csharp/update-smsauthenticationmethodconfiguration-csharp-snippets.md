---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a6c130bd1b047decdc026c14670179ab0bfff02199f5488ccef7eb823443163d
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57378623"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new SmsAuthenticationMethodConfiguration
{
    Id = "Sms",
    State = AuthenticationMethodState.Enabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```