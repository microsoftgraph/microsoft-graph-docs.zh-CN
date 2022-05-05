---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8bbdeadbbd8b5f2932b43b164ffd2cabb41526a8
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65207386"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicyAssignments = await client.api('/policies/roleManagementPolicyAssignments')
    .filter('scopeId eq \'/\' and scopeType eq \'DirectoryRole\' and roleDefinitionId eq \'62e90394-69f5-4237-9190-012177145e10\'')
    .expand('policy($expand=rules)')
    .get();

```