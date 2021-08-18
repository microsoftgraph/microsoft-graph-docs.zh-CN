---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0bbd95caa63d9e38e92baae299aef7d5d6a48dc
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368874"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleManagementPolicyRule = {
  '@odata.type': '#microsoft.graph.unifiedRoleManagementPolicyApprovalRule',
  target: {
    '@odata.type': 'microsoft.graph.unifiedRoleManagementPolicyRuleTarget'
  }
};

await client.api('/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}')
    .version('beta')
    .update(unifiedRoleManagementPolicyRule);

```