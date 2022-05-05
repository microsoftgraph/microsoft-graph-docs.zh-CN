---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9f822d4157c340c28fb724e6387ed9aa7da8a605
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65220320"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let roleManagementPolicyAssignments = await client.api('/policies/roleManagementPolicyAssignments')
    .version('beta')
    .filter('scopeId eq \'/\' and scopeType eq \'Directory\'')
    .get();

```