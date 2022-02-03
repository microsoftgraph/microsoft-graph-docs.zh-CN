---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: df93914fc414c0c7df49236f8959f5fb1dc635f6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62352034"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
    definition: [
    '{\"HomeRealmDiscoveryPolicy\':
     {\'AccelerateToFederatedDomain\':true,
      \'PreferredDomain\':\"federated.example.edu\",
      \'AlternateIdLogin\':{\'Enabled\':true}}}"
  ],
    displayName: 'displayName-value',
    isOrganizationDefault: true
};

await client.api('/policies/homeRealmDiscoveryPolicies')
    .version('beta')
    .post(homeRealmDiscoveryPolicy);

```