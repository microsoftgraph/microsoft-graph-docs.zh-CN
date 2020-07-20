---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d879657b23f66a16260dc651c58364cf1d80c9a4
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44863935"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const homeRealmDiscoveryPolicy = {
  @odata.id:"https://graph.microsoft.com/v1.0/policies/homeRealmDiscoveryPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9"
};

let res = await client.api('/servicePrincipals/{id}/homeRealmDiscoveryPolicies/$ref')
    .post(homeRealmDiscoveryPolicy);

```