---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4fd2e8129573e64b765aa59d92eaee513990aba0
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58368875"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyApprovalRule unifiedRoleManagementPolicyRule = new UnifiedRoleManagementPolicyApprovalRule();
UnifiedRoleManagementPolicyRuleTarget target = new UnifiedRoleManagementPolicyRuleTarget();
unifiedRoleManagementPolicyRule.target = target;

graphClient.policies().roleManagementPolicies("{unifiedRoleManagementPolicyId}").rules("{unifiedRoleManagementPolicyRuleId}")
    .buildRequest()
    .patch(unifiedRoleManagementPolicyRule);

```