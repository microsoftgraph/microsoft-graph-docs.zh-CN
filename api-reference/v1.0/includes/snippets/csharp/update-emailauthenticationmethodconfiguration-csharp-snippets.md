---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 480cce048e7949dcd4a12c6158f9aa90fa9932a79216df9bad9cc2838380ce42
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105567"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var authenticationMethodConfiguration = new EmailAuthenticationMethodConfiguration
{
    AllowExternalIdToUseEmailOtp = ExternalEmailOtpState.Enabled
};

await graphClient.Policies.AuthenticationMethodsPolicy.AuthenticationMethodConfigurations["{authenticationMethodConfiguration-id}"]
    .Request()
    .UpdateAsync(authenticationMethodConfiguration);

```