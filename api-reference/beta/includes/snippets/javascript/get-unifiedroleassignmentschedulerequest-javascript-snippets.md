---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2d1320692e885b6c895a90d12720c5afdf274c8b
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475234"
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