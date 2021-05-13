---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5eba50b8e4c130452d5a2da2c09888776be8c4e3
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474060"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleManagementPolicyAssignment = await client.api('/policies/roleManagementPolicyAssignments/d6e4112f-112f-d6e4-2f11-e4d62f11e4d6')
    .version('beta')
    .get();

```