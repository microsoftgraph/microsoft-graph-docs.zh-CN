---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7f7f24071cf572f1de97651954017d0ab3a0cf95
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092280"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryNoncustodialDataSource()
dataSource := msgraphsdk.NewDataSource()
requestBody.SetDataSource(dataSource)
dataSource.SetAdditionalData(map[string]interface{}{
    "@odata.type": "microsoft.graph.security.siteSource",
}
ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).NoncustodialDataSources().Post(requestBody)


```