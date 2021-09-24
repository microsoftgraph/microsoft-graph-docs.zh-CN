---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bff0500c61ffeb9bf66860942837803133cd6f03
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59508484"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const identityProviderBase = {
    '@odata.type': 'microsoft.graph.samlOrWsFedExternalDomainFederation',
    issuerUri: 'https://contoso.com/issuerUri',
    displayName: 'contoso display name',
    metadataExchangeUri: 'https://contoso.com/metadataExchangeUri',
    passiveSignInUri: 'https://contoso.com/signin',
    preferredAuthenticationProtocol: 'wsFed',
    domains: [
        {
            '@odata.type': 'microsoft.graph.externalDomainName',
            id: 'contoso.com'
        }
    ],
    signingCertificate: 'MIIDADCCAeigAwIBAgIQEX41y8r6'
};

await client.api('/directory/federationConfigurations')
    .version('beta')
    .post(identityProviderBase);

```