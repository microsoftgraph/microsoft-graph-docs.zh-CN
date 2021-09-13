---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 31ca8af82d9747e8c216ff1500d87c3558b9dcf287a27fc3307c789aa98438df
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162342"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
  '@odata.id':'https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref')
    .post(homeRealmDiscoveryPolicy);

```