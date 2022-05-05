---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd7d631336e515629322f84ec21e58fc5c77f507
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211734"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const internalDomainFederation = {
  displayName: 'Contoso name change',  
  federatedIdpMfaBehavior: 'acceptIfMfaDoneByFederatedIdp'
};

await client.api('/domains/contoso.com/federationConfiguration/6601d14b-d113-8f64-fda2-9b5ddda18ecc')
    .version('beta')
    .update(internalDomainFederation);

```