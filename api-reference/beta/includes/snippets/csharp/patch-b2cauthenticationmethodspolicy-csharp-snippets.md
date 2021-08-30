---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 69857bfe5b6cac3dc4d5efa8dd59647f41ac2e20492d47a7a47c32fe7d012be6
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105281"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var b2cAuthenticationMethodsPolicy = new B2cAuthenticationMethodsPolicy
{
    IsEmailPasswordAuthenticationEnabled = false,
    IsUserNameAuthenticationEnabled = true,
    IsPhoneOneTimePasswordAuthenticationEnabled = true
};

await graphClient.Policies.B2cAuthenticationMethodsPolicy
    .Request()
    .UpdateAsync(b2cAuthenticationMethodsPolicy);

```