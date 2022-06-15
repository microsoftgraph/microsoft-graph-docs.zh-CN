---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ebe9bc2c513f58d14861875e98e91aef0735e182
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098794"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewCrossTenantAccessPolicyConfigurationPartner()
tenantId := "3d0f5dec-5d3d-455c-8016-e2af1ae4d31a"
requestBody.SetTenantId(&tenantId)
b2bDirectConnectOutbound := msgraphsdk.NewCrossTenantAccessPolicyB2BSetting()
requestBody.SetB2bDirectConnectOutbound(b2bDirectConnectOutbound)
usersAndGroups := msgraphsdk.NewCrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectOutbound.SetUsersAndGroups(usersAndGroups)
accessType := "blocked"
usersAndGroups.SetAccessType(&accessType)
usersAndGroups.SetTargets( []CrossTenantAccessPolicyTarget {
    msgraphsdk.NewCrossTenantAccessPolicyTarget(),
target := "6f546279-4da5-4b53-a095-09ea0cef9971"
    SetTarget(&target)
targetType := "group"
    SetTargetType(&targetType)
}
b2bDirectConnectInbound := msgraphsdk.NewCrossTenantAccessPolicyB2BSetting()
requestBody.SetB2bDirectConnectInbound(b2bDirectConnectInbound)
applications := msgraphsdk.NewCrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectInbound.SetApplications(applications)
accessType := "allowed"
applications.SetAccessType(&accessType)
applications.SetTargets( []CrossTenantAccessPolicyTarget {
    msgraphsdk.NewCrossTenantAccessPolicyTarget(),
target := "Office365"
    SetTarget(&target)
targetType := "application"
    SetTargetType(&targetType)
}
result, err := graphClient.Policies().CrossTenantAccessPolicy().Partners().Post(requestBody)


```