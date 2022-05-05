---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b669ceb7f2eb8337e53086fb4669b7c81744133
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204419"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

const unifiedRoleManagementPolicyRule = {
    '@odata.type': '#microsoft.graph.unifiedRoleManagementPolicyExpirationRule',
    id: 'Expiration_EndUser_Assignment',
    isExpirationRequired: true,
    maximumDuration: 'PT1H45M',
    target: {
        '@odata.type': 'microsoft.graph.unifiedRoleManagementPolicyRuleTarget',
        caller: 'EndUser',
        operations: [
            'All'
        ],
        level: 'Assignment',
        inheritableSettings: [],
        enforcedSettings: []
    }
};

await client.api('/policies/roleManagementPolicies/DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_200ec19a-09e7-4e7a-9515-cf1ee64b96f9/rules/Expiration_EndUser_Assignment')
    .update(unifiedRoleManagementPolicyRule);

```