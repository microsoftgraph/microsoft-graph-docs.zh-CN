---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c61742cc98ad8c3facd83985ba150c2d8f0266a9
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48965403"
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

graphClient.privilegedAccess("azureResources").roleSettings("5fb5aef8-1081-4b8e-bb16-9d5d0385bab5")
    .buildRequest()
    .patch(governanceRoleSetting);

```