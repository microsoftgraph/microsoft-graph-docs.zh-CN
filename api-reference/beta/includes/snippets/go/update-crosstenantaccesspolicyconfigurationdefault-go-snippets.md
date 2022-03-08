---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 1b51351e48429d73c70e056292162372f07d6276
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335540"
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
graphClient.Policies().CrossTenantAccessPolicy().Default().Patch(options)


```