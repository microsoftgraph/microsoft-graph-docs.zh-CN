---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9241b38ac1c0b258190dcadcac199721a8afb8cb
ms.sourcegitcommit: 496410c1e256aa093eabf27f17e820d9ee91a293
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2020
ms.locfileid: "46566708"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  @odata.type: "microsoft.graph.openIdConnectProvider",
    name: "Login with the Contoso identity provider",
    type: "OpenIDConnect",
    clientId: "56433757-cadd-4135-8431-2c9e3fd68ae8",
    clientSecret: "12345",
    claimsMapping: {
        userId: "myUserId",
        givenName: "myGivenName",
        surname: "mySurname",
        email: "myEmail",
        displayName: "myDisplayName"
    },
    domainHint: "mycustomoidc",
    metadataUrl: "https://mycustomoidc.com/.well-known/openid-configuration",
    responseMode: "form_post",
    responseType: "code",
    scope: "openid"
};

let res = await client.api('/identityProviders')
    .version('beta')
    .post(identityProvider);

```