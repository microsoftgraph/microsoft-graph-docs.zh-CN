---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2e5a822ed6574a2007e226b6beac8ada4de6c408
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103754"
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
options := &msgraphsdk.GovernanceRoleSettingRequestBuilderPatchOptions{
    Body: requestBody,
}
privilegedAccessId := "privilegedAccess-id"
governanceRoleSettingId := "governanceRoleSetting-id"
graphClient.PrivilegedAccessById(&privilegedAccessId).RoleSettingsById(&governanceRoleSettingId).Patch(options)


```