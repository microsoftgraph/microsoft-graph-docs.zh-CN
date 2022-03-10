---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ac26c3fb3c551e1edbb444191f930333924fcde3
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412263"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246",
}
options := &msgraphsdk.NoncustodialDataSourceRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
noncustodialDataSourceId := "noncustodialDataSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).NoncustodialSourcesById(&noncustodialDataSourceId).Post(options)


```