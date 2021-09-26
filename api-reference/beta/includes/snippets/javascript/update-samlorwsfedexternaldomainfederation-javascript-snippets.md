---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44587c7f00765f1898b886b104f4a59d2908a1ad
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59764283"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const samlOrWsFedExternalDomainFederation = {
  displayName: 'Contoso name change',
  issuerUri: 'http://contoso-test.com/adfs/services/trust',
  metadataExchangeUri: null,
  signingCertificate: 'M66C6DCCAdCgAwIBAgIQQ6vYJIVKQ',
  passiveSignInUri: 'https://contoso-test.com/adfs/ls/',
  preferredAuthenticationProtocol: 'wsFed'
};

await client.api('/directory/federationConfigurations/graph.samlOrWsFedExternalDomainFederation/d5a56845-6845-d5a5-4568-a5d54568a5d5')
    .version('beta')
    .update(samlOrWsFedExternalDomainFederation);

```