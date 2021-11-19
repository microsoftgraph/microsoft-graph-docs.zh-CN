---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b8ed4f06d1930da1759249d0e7a12a6acc9527e5
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085602"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewDataSource()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.ediscovery.siteSource",
}
options := &msgraphsdk.AdditionalSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).AdditionalSources().Post(options)


```