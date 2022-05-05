---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 344e1616548c5e5d2fffe34e9d738651f8e7b544
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/05/2022
ms.locfileid: "65202392"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedAdminAccessAssignment()
accessDetails := msgraphsdk.NewDelegatedAdminAccessDetails()
requestBody.SetAccessDetails(accessDetails)
accessDetails.SetUnifiedRoles( []UnifiedRole {
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "88d8e3e3-8f55-4a1e-953a-9b9898b8876b",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "44367163-eba1-44c3-98af-f5787879f96a",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
    }
}
headers := map[string]string{
    "If-Match": "W/"JyI0NzAwNjg0NS0wMDAwLTE5MDAtMDAwMC02MGY0Yjg4MzAwMDAiJw==""
}
options := &msgraphsdk.DelegatedAdminAccessAssignmentRequestBuilderPatchOptions{
    Body: requestBody,
    H: headers,
}
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
delegatedAdminAccessAssignmentId := "delegatedAdminAccessAssignment-id"
graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).AccessAssignmentsById(&delegatedAdminAccessAssignmentId).Patch(options)


```