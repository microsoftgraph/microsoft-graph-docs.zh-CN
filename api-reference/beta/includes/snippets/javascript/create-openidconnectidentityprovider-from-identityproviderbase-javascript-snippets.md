---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0ab4d95e7768dd4bfc05d7795cea4eb807927e9ed8782ac912fe6f9fe7dd15b0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105749"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
  '@odata.type': 'microsoft.graph.openIdConnectIdentityProvider',
    displayName: 'Login with the Contoso identity provider',
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

await client.api('/identity/identityProviders')
    .version('beta')
    .post(identityProviderBase);

```