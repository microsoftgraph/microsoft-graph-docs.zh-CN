---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4a08428f3d4b385f34f6bac4056bc8dcd9c53df2
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52475270"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleEligibilityScheduleRequest = await client.api('/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}')
    .version('beta')
    .get();

```