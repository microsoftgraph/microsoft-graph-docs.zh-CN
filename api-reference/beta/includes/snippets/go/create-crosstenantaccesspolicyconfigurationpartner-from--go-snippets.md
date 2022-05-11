---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 00d3eb726fcbbe97d36c1b30a2d92318100b746b
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326389"
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
    SetAdditionalData(map[string]interface{}{
        "target": "6f546279-4da5-4b53-a095-09ea0cef9971",
        "targetType": "group",
    }
}
b2bDirectConnectInbound := msgraphsdk.NewCrossTenantAccessPolicyB2BSetting()
requestBody.SetB2bDirectConnectInbound(b2bDirectConnectInbound)
applications := msgraphsdk.NewCrossTenantAccessPolicyTargetConfiguration()
b2bDirectConnectInbound.SetApplications(applications)
accessType := "allowed"
applications.SetAccessType(&accessType)
applications.SetTargets( []CrossTenantAccessPolicyTarget {
    msgraphsdk.NewCrossTenantAccessPolicyTarget(),
    SetAdditionalData(map[string]interface{}{
        "target": "Office365",
        "targetType": "application",
    }
}
result, err := graphClient.Policies().CrossTenantAccessPolicy().Partners().Post(requestBody)


```