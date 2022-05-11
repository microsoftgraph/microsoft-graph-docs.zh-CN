---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 000c70cec09237156fde777d9c095dd5a31a090b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327470"
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
graphClient.Policies().CrossTenantAccessPolicy().Default().Patch(requestBody)


```