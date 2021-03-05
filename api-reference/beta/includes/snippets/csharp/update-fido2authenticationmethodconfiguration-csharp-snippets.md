---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 861a867c57d37e0237d6ab9d6e0f0f7fab06d2c6
ms.sourcegitcommit: d014f72cf2cd130bedb02651092c0be12967b679
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50471064"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new Fido2AuthenticationMethodConfiguration
{
    State = AuthenticationMethodState.Enabled,
    IsAttestationEnforced = true
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["fido2"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```