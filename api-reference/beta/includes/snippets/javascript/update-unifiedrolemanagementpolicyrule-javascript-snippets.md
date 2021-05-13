---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e0a1e9f7d82defc19e99cb0c95b9cc22ae98f0aa
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474248"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleManagementPolicyRule = {
  '@odata.type': '#microsoft.graph.unifiedRoleManagementPolicyRule',
  target: {
    '@odata.type': 'microsoft.graph.unifiedRoleManagementPolicyRuleTarget'
  }
};

await client.api('/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}')
    .version('beta')
    .update(unifiedRoleManagementPolicyRule);

```