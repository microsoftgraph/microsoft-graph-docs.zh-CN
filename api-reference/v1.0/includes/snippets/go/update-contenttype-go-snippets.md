---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c439d9421b799ab0f23867725f2ced6be667b454
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65328344"
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
siteId := "site-id"
contentTypeId := "contentType-id"
graphClient.SitesById(&siteId).ContentTypesById(&contentTypeId).Patch(requestBody)


```