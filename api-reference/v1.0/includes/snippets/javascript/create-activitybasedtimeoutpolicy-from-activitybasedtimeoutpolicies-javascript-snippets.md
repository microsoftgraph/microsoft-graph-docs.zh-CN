---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: bb538ad31719dc843b60051513dbbefb83768c7c
ms.sourcegitcommit: 5575e6607817ba23ceb0b01e2f5fc81e58bdcd1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43806304"
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
  isOrganizationDefault: true
};

let res = await client.api('/policies/activityBasedTimeoutPolicies')
    .post(activityBasedTimeoutPolicy);

```