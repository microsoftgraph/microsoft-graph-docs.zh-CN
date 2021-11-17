---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 17a1070810c988b0e2e669d470e78fb7de92b782
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60994180"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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