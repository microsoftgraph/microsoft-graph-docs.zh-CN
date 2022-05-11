---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 44587c7f00765f1898b886b104f4a59d2908a1ad
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65315247"
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