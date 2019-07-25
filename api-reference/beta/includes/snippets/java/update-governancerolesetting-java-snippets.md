---
description: 自动生成的文件。 不修改
ms.openlocfilehash: d3c019eafd36d72bd4c221ae92fee6ca6cf665b9
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35859085"
---
```java

IGraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

GovernanceRoleSetting governanceRoleSetting = new GovernanceRoleSetting();
LinkedList<GovernanceRuleSetting> adminEligibleSettingsList = new LinkedList<GovernanceRuleSetting>();
GovernanceRuleSetting adminEligibleSettings = new GovernanceRuleSetting();
adminEligibleSettings.ruleIdentifier = "ExpirationRule";
adminEligibleSettings.setting = "{\"permanentAssignment\":false,\"maximumGrantPeriodInMinutes\":129600}";
adminEligibleSettingsList.add(adminEligibleSettings);
governanceRoleSetting.adminEligibleSettings = adminEligibleSettingsList;

graphClient.privilegedAccess("pimforazurerbac").roleSettings("5fb5aef8-1081-4b8e-bb16-9d5d0385bab5")
    .buildRequest()
    .patch(governanceRoleSetting);

```