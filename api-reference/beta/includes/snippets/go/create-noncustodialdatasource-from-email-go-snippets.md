---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 55b8eba397f0c4a2ce062818c51303a35351ba23
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61102184"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewNoncustodialDataSource()
applyHoldToSource := true
requestBody.SetApplyHoldToSource(&applyHoldToSource)
dataSource := msgraphsdk.NewDataSource()
requestBody.SetDataSource(dataSource)
dataSource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.ediscovery.userSource",
    "email": "adelev@contoso.com",
}
options := &msgraphsdk.NoncustodialDataSourcesRequestBuilderPostOptions{
    Body: requestBody,
}
caseId := "case-id"
result, err := graphClient.Compliance().Ediscovery().CasesById(&caseId).NoncustodialDataSources().Post(options)


```