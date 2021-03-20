---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 618477c55818abe7397d9827b98fa32efe45bc8f
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50970676"
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