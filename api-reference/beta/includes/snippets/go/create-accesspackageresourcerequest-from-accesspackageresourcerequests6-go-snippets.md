---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 27aa64b1fec2f3536bb3f8e7353848b949577993
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098796"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageResourceRequest()
catalogId := "26ac0c0a-08bc-4a7b-a313-839f58044ba5"
requestBody.SetCatalogId(&catalogId)
requestType := "AdminAdd"
requestBody.SetRequestType(&requestType)
justification := ""
requestBody.SetJustification(&justification)
accessPackageResource := msgraphsdk.NewAccessPackageResource()
requestBody.SetAccessPackageResource(accessPackageResource)
displayName := "Faculty cafeteria ordering"
accessPackageResource.SetDisplayName(&displayName)
description := "Example application"
accessPackageResource.SetDescription(&description)
url := "https://myapps.microsoft.com/example.com/signin/Faculty%20cafeteria%20ordering/f1e3b407-942d-4934-9a3f-cef1975cb988/"
accessPackageResource.SetUrl(&url)
resourceType := "Application"
accessPackageResource.SetResourceType(&resourceType)
originId := "2f1099a6-d4fc-4cc9-a0ef-ddd3f1bf0b7e"
accessPackageResource.SetOriginId(&originId)
originSystem := "AadApplication"
accessPackageResource.SetOriginSystem(&originSystem)
accessPackageResource.SetAttributes( []AccessPackageResourceAttribute {
    msgraphsdk.NewAccessPackageResourceAttribute(),
attributeName := "extension_2b676109c7c74ae2b41549205f1947ed_personalTitle"
    SetAttributeName(&attributeName)
isEditable := true
    SetIsEditable(&isEditable)
isPersistedOnAssignmentRemoval := true
    SetIsPersistedOnAssignmentRemoval(&isPersistedOnAssignmentRemoval)
attributeSource := msgraphsdk.NewAccessPackageResourceAttributeSource()
    SetAttributeSource(attributeSource)
    attributeSource.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageResourceAttributeQuestion",
    }
attributeDestination := msgraphsdk.NewAccessPackageResourceAttributeDestination()
    SetAttributeDestination(attributeDestination)
    attributeDestination.SetAdditionalData(map[string]interface{}{
        "@odata.type": "#microsoft.graph.accessPackageUserDirectoryAttributeStore",
    }
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageResourceRequests().Post(requestBody)


```