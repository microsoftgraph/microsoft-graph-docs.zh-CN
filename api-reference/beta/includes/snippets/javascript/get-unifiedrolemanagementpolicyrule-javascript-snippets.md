---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9a4cf9036ab568820aca0f34f25ea05793a57e187a65df5e5715610301b523d5
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57105707"
---
```javascript

const options = {
    authProvider,
};

const client = Client.init(options);

let unifiedRoleManagementPolicyRule = await client.api('/policies/roleManagementPolicies/{unifiedRoleManagementPolicyId}/rules/{unifiedRoleManagementPolicyRuleId}')
    .version('beta')
    .get();

```