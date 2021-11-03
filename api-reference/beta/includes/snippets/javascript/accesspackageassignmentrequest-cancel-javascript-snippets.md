---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09c2fe4021d9c1586e29ea2e43146fc5c9b722657f0c0a951719be41c31cb8f1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "56902804"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const cancel = {
  id: 'request-id',
  requestStatus: 'cancelled'
};

await client.api('/identityGovernance/entitlementManagement/accessPackageAssignmentRequests/{id}/cancel')
    .version('beta')
    .post(cancel);

```