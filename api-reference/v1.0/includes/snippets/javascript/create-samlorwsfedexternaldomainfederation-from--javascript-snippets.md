---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bff0500c61ffeb9bf66860942837803133cd6f03
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315726"
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