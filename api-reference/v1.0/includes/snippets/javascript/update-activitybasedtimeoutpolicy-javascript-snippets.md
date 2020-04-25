---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b93fc37eeee7cf28d374a93760214d88519d8a4
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806243"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const activityBasedTimeoutPolicy = {
  definition: [
    "definition-value"
  ],
  displayName: "displayName-value",
  isOrganizationDefault: true,
  type: "type-value"
};

let res = await client.api('/policies/activityBasedTimeoutPolicies/{id}')
    .update(activityBasedTimeoutPolicy);

```