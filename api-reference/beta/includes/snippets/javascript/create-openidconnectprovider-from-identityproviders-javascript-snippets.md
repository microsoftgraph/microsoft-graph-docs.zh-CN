---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0a9fbac45f9221313245baa9ff0f73324ab1b77f
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50786009"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProvider = {
  '@odata.type': 'microsoft.graph.openIdConnectProvider',
    name: 'Login with the Contoso identity provider',
    type: 'OpenIDConnect',
    clientId: '56433757-cadd-4135-8431-2c9e3fd68ae8',
    clientSecret: '12345',
    claimsMapping: {
        userId: 'myUserId',
        givenName: 'myGivenName',
        surname: 'mySurname',
        email: 'myEmail',
        displayName: 'myDisplayName'
    },
    domainHint: 'mycustomoidc',
    metadataUrl: 'https://mycustomoidc.com/.well-known/openid-configuration',
    responseMode: 'form_post',
    responseType: 'code',
    scope: 'openid'
};

await client.api('/identityProviders')
    .version('beta')
    .post(identityProvider);

```