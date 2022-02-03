---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0f098c7af8097af3403ab50506894478383cb3e6
ms.sourcegitcommit: 25acfa7d0153336c9a35d30a1dd422aeadc1342c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/03/2022
ms.locfileid: "62346394"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
    '@odata.id': 'https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/6c6f154f-cb39-4ff9-bf5b-62d5ad585cde'
};

await client.api('/servicePrincipals/19c308f2-e088-464d-8ccb-7137b7bab660/homeRealmDiscoveryPolicies/$ref')
    .version('beta')
    .post(homeRealmDiscoveryPolicy);

```