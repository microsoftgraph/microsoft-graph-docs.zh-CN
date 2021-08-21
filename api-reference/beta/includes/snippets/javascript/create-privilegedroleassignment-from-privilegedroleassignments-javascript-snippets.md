---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e3359ac43184462638b1d69707f03854dd5b64015dc12603c7c434e85965dbd
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57279264"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const privilegedRoleAssignment = {
  userId: 'userId-value',
  roleId: 'roleId-value'
};

await client.api('/privilegedRoleAssignments')
    .version('beta')
    .post(privilegedRoleAssignment);

```