---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 556631fbd3fa54aa9d6cbfe97ac7504efc4e238b
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202366"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const internalDomainFederation = {
  '@odata.type': '#microsoft.graph.internalDomainFederation',
  displayName: 'Contoso',
  issuerUri: 'http://contoso.com/adfs/services/trust',
  metadataExchangeUri: 'https://sts.contoso.com/adfs/services/trust/mex',
  signingCertificate: 'MIIE3jCCAsagAwIBAgIQQcyDaZz3MI',
  passiveSignInUri: 'https://sts.contoso.com/adfs/ls',
  preferredAuthenticationProtocol: 'wsFed',
  activeSignInUri: 'https://sts.contoso.com/adfs/services/trust/2005/usernamemixed',
  signOutUri: 'https://sts.contoso.com/adfs/ls',
  promptLoginBehavior: 'nativeSupport',
  isSignedAuthenticationRequestRequired: true,
  nextSigningCertificate: 'MIIE3jCCAsagAwIBAgIQQcyDaZz3MI',
  federatedIdpMfaBehavior: 'rejectMfaByFederatedIdp'
};

await client.api('/domains/contoso.com/federationConfiguration')
    .version('beta')
    .post(internalDomainFederation);

```