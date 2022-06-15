---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4c31a4729e43dba9363c1b070667aede6a2511a9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098770"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGovernanceRoleSetting()
requestBody.SetAdminEligibleSettings( []GovernanceRuleSetting {
    msgraphsdk.NewGovernanceRuleSetting(),
ruleIdentifier := "ExpirationRule"
    SetRuleIdentifier(&ruleIdentifier)
setting := "{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}"
    SetSetting(&setting)
}
privilegedAccessId := "privilegedAccess-id"
governanceRoleSettingId := "governanceRoleSetting-id"
graphClient.PrivilegedAccessById(&privilegedAccessId).RoleSettingsById(&governanceRoleSettingId).Patch(requestBody)


```