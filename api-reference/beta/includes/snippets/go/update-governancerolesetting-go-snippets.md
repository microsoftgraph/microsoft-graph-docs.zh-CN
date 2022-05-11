---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0aa435cfda18ffcb12b463f3c7c75d0ccb2b0d7e
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328156"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewGovernanceRoleSetting()
requestBody.SetAdminEligibleSettings( []GovernanceRuleSetting {
    msgraphsdk.NewGovernanceRuleSetting(),
    SetAdditionalData(map[string]interface{}{
        "ruleIdentifier": "ExpirationRule",
        "setting": "{"permanentAssignment":false,"maximumGrantPeriodInMinutes":129600}",
    }
}
privilegedAccessId := "privilegedAccess-id"
governanceRoleSettingId := "governanceRoleSetting-id"
graphClient.PrivilegedAccessById(&privilegedAccessId).RoleSettingsById(&governanceRoleSettingId).Patch(requestBody)


```