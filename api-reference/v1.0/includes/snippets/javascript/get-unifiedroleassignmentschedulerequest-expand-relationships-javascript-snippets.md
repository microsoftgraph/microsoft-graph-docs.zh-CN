---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 09f4a1e6a0760af6fc71ce299709ae64caa6dd8c
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65205068"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleAssignmentScheduleRequest = await client.api('/roleManagement/directory/roleAssignmentScheduleRequests/95c690fb-3eb3-4942-a03f-4524aed6f31e')
    .expand('roleDefinitionId')
    .select('principalId,action,roleDefinitionId')
    .get();

```