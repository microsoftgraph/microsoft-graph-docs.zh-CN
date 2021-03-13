---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ecf2bcfa1f94fbfc2e8cb459d489390cc97aeb90
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50805539"
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

await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .version('beta')
    .update(activityBasedTimeoutPolicy);

```