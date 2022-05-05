---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 08c9c168fa20a89386ce368720d20d0882ade38f
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204672"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleManagementPolicy = await client.api('/policies/roleManagementPolicies/DirectoryRole_cab01047-8ad9-4792-8e42-569340767f1b_70c808b5-0d35-4863-a0ba-07888e99d448')
    .expand('effectiveRules,rules')
    .get();

```