---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7e8af165a4e12670e17aefd77d6dd583b6afc9dc7610e7d250f17ea1808ea6ec
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902602"
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