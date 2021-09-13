---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8f891c7d76472370f50db5198d5b4ba3ad338dcad5132b5a7d5f43e5f43bba6a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57409385"
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
    .post(activityBasedTimeoutPolicy);

```