---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2ed827f9de81311c208b13d71f07f545ea64b5b6
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65204422"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

UnifiedRoleManagementPolicyExpirationRule unifiedRoleManagementPolicyRule = new UnifiedRoleManagementPolicyExpirationRule();
unifiedRoleManagementPolicyRule.id = "Expiration_EndUser_Assignment";
unifiedRoleManagementPolicyRule.isExpirationRequired = true;
unifiedRoleManagementPolicyRule.maximumDuration = DatatypeFactory.newInstance().newDuration("PT1H45M");
UnifiedRoleManagementPolicyRuleTarget target = new UnifiedRoleManagementPolicyRuleTarget();
target.caller = "EndUser";
LinkedList<UnifiedRoleManagementPolicyRuleTargetOperations> operationsList = new LinkedList<UnifiedRoleManagementPolicyRuleTargetOperations>();
operationsList.add(UnifiedRoleManagementPolicyRuleTargetOperations.ALL);
target.operations = operationsList;
target.level = "Assignment";
LinkedList<String> inheritableSettingsList = new LinkedList<String>();
target.inheritableSettings = inheritableSettingsList;
LinkedList<String> enforcedSettingsList = new LinkedList<String>();
target.enforcedSettings = enforcedSettingsList;
unifiedRoleManagementPolicyRule.target = target;

graphClient.policies().roleManagementPolicies("DirectoryRole_84841066-274d-4ec0-a5c1-276be684bdd3_200ec19a-09e7-4e7a-9515-cf1ee64b96f9").rules("Expiration_EndUser_Assignment")
    .buildRequest()
    .patch(unifiedRoleManagementPolicyRule);

```