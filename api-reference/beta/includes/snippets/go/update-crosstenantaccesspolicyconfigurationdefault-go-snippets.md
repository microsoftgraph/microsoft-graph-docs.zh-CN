---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce07a22784e7ad01411af4b773d61645f63ac643
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098790"
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
target := "0be493dc-cb56-4a53-936f-9cf64410b8b0"
    SetTarget(&target)
targetType := "group"
    SetTargetType(&targetType)
}
applications := msgraphsdk.NewCrossTenantAccessPolicyTargetConfiguration()
b2bCollaborationOutbound.SetApplications(applications)
accessType := "blocked"
applications.SetAccessType(&accessType)
applications.SetTargets( []CrossTenantAccessPolicyTarget {
    msgraphsdk.NewCrossTenantAccessPolicyTarget(),
target := "AllApplications"
    SetTarget(&target)
targetType := "application"
    SetTargetType(&targetType)
}
graphClient.Policies().CrossTenantAccessPolicy().Default().Patch(requestBody)


```