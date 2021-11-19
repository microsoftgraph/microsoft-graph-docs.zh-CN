---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8b21d62748eb03bc97dd0d6e5b591372d8abe40d
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61103646"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SourceCollectionRequestBuilderGetQueryParameters{
    Expand: "addToReviewSetOperation,custodianSources,lastEstimateStatisticsOperation",
}
options := &msgraphsdk.SourceCollectionRequestBuilderGetOptions{
    Q: requestParameters,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).Get(options)


```