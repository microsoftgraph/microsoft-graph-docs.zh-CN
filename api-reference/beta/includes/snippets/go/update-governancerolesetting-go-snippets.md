---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 6d86bb34629d7137f3a6b144a50e4241c6a3ab2b
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61028523"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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