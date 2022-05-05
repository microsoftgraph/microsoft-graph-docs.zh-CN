---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d4f5e81fee723ddad3e24ff0c3300b6c3a9e99ad
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205091"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentScheduleRequest = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/95c690fb-3eb3-4942-a03f-4524aed6f31e')
    .get();

```