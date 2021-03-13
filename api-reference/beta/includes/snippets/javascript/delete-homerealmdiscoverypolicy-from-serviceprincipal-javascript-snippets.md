---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cb7310bb66a2a5b856938dc65b9204f0fe6a6400
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50809244"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

await client.api('/servicePrincipals/{servicePrincipalId}/homeRealmDiscoveryPolicies/{policyId}/$ref')
    .version('beta')
    .delete();

```