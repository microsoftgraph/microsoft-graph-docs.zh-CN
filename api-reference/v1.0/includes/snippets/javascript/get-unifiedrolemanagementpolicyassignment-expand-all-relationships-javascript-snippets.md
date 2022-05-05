---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fdc27309d7f52d430fe42c6d5543822ea6e3dc90
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204505"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleManagementPolicyAssignment = await client.api('/policies/roleManagementPolicyAssignments/Directory_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448_62e90394-69f5-4237-9190-012177145e10')
    .expand('policy($expand=rules)')
    .get();

```