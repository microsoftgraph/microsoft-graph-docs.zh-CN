---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 681c7226fbae68044f79ee25a8a8550160765bc3
ms.sourcegitcommit: e440d855f1106390d842905d97ceb16f143db2e5
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/29/2021
ms.locfileid: "52081507"
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