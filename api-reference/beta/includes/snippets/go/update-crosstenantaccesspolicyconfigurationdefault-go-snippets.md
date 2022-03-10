---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: a7397e7aeb7f40b28c79ddd10ba3bc092e89794a
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412386"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicyConfigurationDefault()
b2bCollaborationOutbound := msgraphsdk.NewCrossTenantAccessPolicyB2BSetting()
requestBody.SetB2bCollaborationOutbound(b2bCollaborationOutbound)
usersAndGroups := msgraphsdk.NewCrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutbound.SetUsersAndGroups(usersAndGroups)
accessType := "blocked"
usersAndGroups.SetAccessType(&accessType)
usersAndGroups.SetTargets( []CrossTenantAccessPolicyTarget {
    msgraphsdk.NewCrossTenantAccessPolicyTarget(),
    SetAdditionalData(map[string]interface{}{
        "target": "0be493dc-cb56-4a53-936f-9cf64410b8b0",
        "targetType": "group",
    }
}
applications := msgraphsdk.NewCrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutbound.SetApplications(applications)
accessType := "blocked"
applications.SetAccessType(&accessType)
applications.SetTargets( []CrossTenantAccessPolicyTarget {
    msgraphsdk.NewCrossTenantAccessPolicyTarget(),
    SetAdditionalData(map[string]interface{}{
        "target": "AllApplications",
        "targetType": "application",
    }
}
options := &msgraphsdk.DefaultRequestBuilderPatchOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().CrossTenantAccessPolicy().Default().Patch(options)


```