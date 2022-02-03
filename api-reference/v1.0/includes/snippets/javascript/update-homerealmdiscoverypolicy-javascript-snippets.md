---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bf7266f8e8c3d6d158de24f2848ee12a159bc0b4
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62350477"
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
    displayName: 'Contoso default HRD Policy'
};

await client.api('/policies/homeRealmDiscoveryPolicies/{id}')
    .update(homeRealmDiscoveryPolicy);

```