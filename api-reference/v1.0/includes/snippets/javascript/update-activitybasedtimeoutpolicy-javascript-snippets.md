---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ad4ebe4cfd4264b70757459bebf7b78a39881d5e56ada9aaa82a247e9fa38f56
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57163033"
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
    .update(activityBasedTimeoutPolicy);

```