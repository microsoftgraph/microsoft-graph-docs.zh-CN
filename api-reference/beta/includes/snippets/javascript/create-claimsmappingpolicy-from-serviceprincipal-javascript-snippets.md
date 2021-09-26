---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4f01a2e6a77e1922760fe34901e04096f1546cf3
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59767179"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
  '@odata.id':'https://graph.microsoft.com/beta/policies/claimsMappingPolicies/cd3d9b57-0aee-4f25-8ee3-ac74ef5986a9'
};

await client.api('/servicePrincipals/{servicePrincipal-id}/claimsMappingPolicies/$ref')
    .version('beta')
    .post(claimsMappingPolicy);

```