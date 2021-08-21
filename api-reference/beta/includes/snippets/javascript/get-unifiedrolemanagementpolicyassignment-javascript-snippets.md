---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c8d36195478b0fc1c62e316c3c4a05fda6ed994e70f1e6e575208fc94ff6b58
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57162432"
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