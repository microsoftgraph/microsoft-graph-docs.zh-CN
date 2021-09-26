---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f5e18173015c94331b314cc0214070d7dca4ed94
ms.sourcegitcommit: 08e9b0bac39c1b1d2c8a79539d24aaa93364baf2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/24/2021
ms.locfileid: "59763806"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const claimsMappingPolicy = {
    displayName: 'UpdateClaimsPolicy'
};

await client.api('/policies/claimsMappingPolicies/{id}')
    .version('beta')
    .update(claimsMappingPolicy);

```