---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6118aa3b8f724cce1633fe1513ec322e7acf1d9cdb64843040699de89001809e
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162730"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies')
    .version('beta')
    .post(homeRealmDiscoveryPolicy);

```