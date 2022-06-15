---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 8c246e880617221721f958a88cb422c839b24bf3
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093602"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.FilesRequestBuilderGetQueryParameters{
    Top: 5,
}
options := &msgraphsdk.FilesRequestBuilderGetRequestConfiguration{
    QueryParameters: requestParameters,
}
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewSetId := "ediscoveryReviewSet-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).ReviewSetsById(&ediscoveryReviewSetId).Files().GetWithRequestConfigurationAndResponseHandler(options, nil)


```