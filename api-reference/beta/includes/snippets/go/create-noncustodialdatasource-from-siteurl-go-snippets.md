---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ef874e8826dc56601d6fbd544d4d18df46907d8f
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327192"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNoncustodialDataSource()
applyHoldToSource := false
requestBody.SetApplyHoldToSource(&applyHoldToSource)
dataSource := msgraphsdk.NewDataSource()
requestBody.SetDataSource(dataSource)
dataSource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.ediscovery.siteSource",
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSources().Post(requestBody)


```