---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d5572f01a1c04c99de811136350b47c8da5248a5
ms.sourcegitcommit: 77d2ab5018371f153d47cc1cd25f9dcbaca28a95
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/08/2022
ms.locfileid: "63335834"
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
options := &msgraphsdk.PartnersRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.Policies().CrossTenantAccessPolicy().Partners().Post(options)


```