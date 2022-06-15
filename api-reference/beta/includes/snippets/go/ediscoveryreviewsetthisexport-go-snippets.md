---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b2f0f86d603ac74862d921c0cd464aa4b2267ddc
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66092383"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.New()
outputName := "Export via API"
requestBody.SetOutputName(&outputName)
description := "Export for the Contoso investigation"
requestBody.SetDescription(&description)
exportOptions := "originalFiles,fileInfo,tags"
requestBody.SetExportOptions(&exportOptions)
exportStructure := "directory"
requestBody.SetExportStructure(&exportStructure)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewSetId := "ediscoveryReviewSet-id"
graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).ReviewSetsById(&ediscoveryReviewSetId).Export(ediscoveryCase-id, ediscoveryReviewSet-id).Post(requestBody)


```