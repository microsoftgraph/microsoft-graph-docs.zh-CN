---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd5b27f1ab371e6997030122853dc6df3539680c
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327546"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
requestBody.SetAdditionalData(map[string]interface{}{
    "@odata.id": "https://canary.graph.microsoft.com/testprodbetancsdsaslist/compliance/ediscovery/cases/06d52284-ed81-49b8-904a-b863d3164731/noncustodialDataSources/39383530323537383742433232433246",
}
caseId := "case-id"
sourceCollectionId := "sourceCollection-id"
noncustodialDataSourceId := "noncustodialDataSource-id"
graphClient.Compliance().Ediscovery().CasesById(&caseId).SourceCollectionsById(&sourceCollectionId).NoncustodialSourcesById(&noncustodialDataSourceId).Post(requestBody)


```