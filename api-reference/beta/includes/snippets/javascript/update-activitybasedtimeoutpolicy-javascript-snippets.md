---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 15585d3d21ff804483ac0963330611ee15e8c5bacdb65892a26f80184e8dc68a
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57104097"
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