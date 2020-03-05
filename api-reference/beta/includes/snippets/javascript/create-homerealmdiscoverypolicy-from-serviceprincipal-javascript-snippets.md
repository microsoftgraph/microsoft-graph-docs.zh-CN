---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1676961dc0367bf37b23d0e515cea4052692df59
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41476569"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicies = {
  @odata.id:"https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies')
    .version('beta')
    .post(homeRealmDiscoveryPolicies);

```