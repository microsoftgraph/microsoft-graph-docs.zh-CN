---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d0cf887edd4ca027486c1326ba379f7c8155d1beb2283b55ef0edfc68d683c3f
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "57329044"
---
```java

GraphServiceClient graphClient = GraphServiceClient.builder().authenticationProvider( authProvider ).buildClient();

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