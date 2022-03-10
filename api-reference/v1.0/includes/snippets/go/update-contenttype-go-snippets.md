---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: cc710550362e331f04702de7fc1f3cd0d9ce63e7
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411870"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewContentType()
name := "updatedCt"
requestBody.SetName(&name)
documentSet := msgraphsdk.NewDocumentSet()
requestBody.SetDocumentSet(documentSet)
shouldPrefixNameToFile := true
documentSet.SetShouldPrefixNameToFile(&shouldPrefixNameToFile)
documentSet.SetAllowedContentTypes( []ContentTypeInfo {
    msgraphsdk.NewContentTypeInfo(),
    SetAdditionalData(map[string]interface{}{
        "id": "0x0101",
        "name": "Document",
    }
}
documentSet.SetDefaultContents( []DocumentSetContent {
    msgraphsdk.NewDocumentSetContent(),
    SetAdditionalData(map[string]interface{}{
        "fileName": "a.txt",
    }
    msgraphsdk.NewDocumentSetContent(),
    SetAdditionalData(map[string]interface{}{
        "fileName": "b.txt",
    }
}
documentSet.SetSharedColumns( []ColumnDefinition {
    msgraphsdk.NewColumnDefinition(),
    SetAdditionalData(map[string]interface{}{
        "name": "Description",
        "id": "cbb92da4-fd46-4c7d-af6c-3128c2a5576e",
    }
    msgraphsdk.NewColumnDefinition(),
    SetAdditionalData(map[string]interface{}{
        "name": "Address",
        "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50",
    }
}
documentSet.SetWelcomePageColumns( []ColumnDefinition {
    msgraphsdk.NewColumnDefinition(),
    SetAdditionalData(map[string]interface{}{
        "name": "Address",
        "id": "fc2e188e-ba91-48c9-9dd3-16431afddd50",
    }
}
options := &msgraphsdk.ContentTypeRequestBuilderPatchOptions{
    Body: requestBody,
}
siteId := "site-id"
contentTypeId := "contentType-id"
result, err := graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Patch(options)


```