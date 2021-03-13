---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 76da9e4ce694f3e1dca171684a1b9e67fa17b270
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50792732"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const activityBasedTimeoutPolicy = {
  definition: [
    'definition-value'
  ],
  displayName: 'displayName-value',
  isOrganizationDefault: true
};

await client.api('/policies/activityBasedTimeoutPolicies')
    .version('beta')
    .post(activityBasedTimeoutPolicy);

```