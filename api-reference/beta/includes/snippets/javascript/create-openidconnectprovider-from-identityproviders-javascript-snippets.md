---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 03c84c30fbf62debe3277aa400e056b742647ea834f83b53e1ba430cd4631833
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57278958"
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