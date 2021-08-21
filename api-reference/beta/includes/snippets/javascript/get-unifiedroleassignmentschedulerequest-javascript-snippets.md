---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 67315614013d80a08c1bee55332ac15d07ae9f00598e748a3e5e6c2fc85969a0
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57158435"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentScheduleRequest = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/{unifiedRoleAssignmentScheduleRequestsId}')
    .version('beta')
    .get();

```