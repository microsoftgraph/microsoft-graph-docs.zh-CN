---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 985d7d1d21690bc5ef0c89bc9b5a76f307385acb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095880"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
outputName := "Export reviewset query via API"
requestBody.SetOutputName(&outputName)
description := "Export for the Contoso investigation 2"
requestBody.SetDescription(&description)
exportOptions := "originalFiles,fileInfo,tags"
requestBody.SetExportOptions(&exportOptions)
exportStructure := "directory"
requestBody.SetExportStructure(&exportStructure)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewSetId := "ediscoveryReviewSet-id"
ediscoveryReviewSetQueryId := "ediscoveryReviewSetQuery-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).ReviewSetsById(&ediscoveryReviewSetId).QueriesById(&ediscoveryReviewSetQueryId).Export(ediscoveryCase-id, ediscoveryReviewSet-id, ediscoveryReviewSetQuery-id).Post(requestBody)


```