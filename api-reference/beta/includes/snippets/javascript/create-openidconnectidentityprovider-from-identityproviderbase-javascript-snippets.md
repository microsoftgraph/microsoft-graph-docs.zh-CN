---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 87c10d8e177cad3548151dd13b3b8720b0d046ac
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921316"
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