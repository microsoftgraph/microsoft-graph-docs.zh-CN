---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b4f52e2662691c69f72bb2f692ca971a24f5e164590d4e0f19617b765577217c
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162483"
---
```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var identityProvider = new IdentityProvider
{
    ResponseType = OpenIdConnectResponseTypes.Id_token
};

await graphClient.IdentityProviders["{identityProvider-id}"]
    .Request()
    .UpdateAsync(identityProvider);

```