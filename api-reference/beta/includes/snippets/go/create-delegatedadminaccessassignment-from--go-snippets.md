---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ba09636810a7808c4ba5cf89c6b26d3852129aeb
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328509"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDelegatedAdminAccessAssignment()
accessContainer := msgraphsdk.NewDelegatedAdminAccessContainer()
requestBody.SetAccessContainer(accessContainer)
accessContainerId := "869713c9-0b28-4d08-8949-ae07ae1bf528"
accessContainer.SetAccessContainerId(&accessContainerId)
accessContainerType := "securityGroup"
accessContainer.SetAccessContainerType(&accessContainerType)
accessDetails := msgraphsdk.NewDelegatedAdminAccessDetails()
requestBody.SetAccessDetails(accessDetails)
accessDetails.SetUnifiedRoles( []UnifiedRole {
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "29232cdf-9323-42fd-ade2-1d097af3e4de",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "f2ef992c-3afb-46b9-b7cf-a126ee74c451",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "729827e3-9c14-49f7-bb1b-9608f156bbb8",
    }
    msgraphsdk.NewUnifiedRole(),
    SetAdditionalData(map[string]interface{}{
        "roleDefinitionId": "3a2c62db-5318-420d-8d74-23affee5d9d5",
    }
}
delegatedAdminRelationshipId := "delegatedAdminRelationship-id"
result, err := graphClient.TenantRelationships().DelegatedAdminRelationshipsById(&delegatedAdminRelationshipId).AccessAssignments().Post(requestBody)


```