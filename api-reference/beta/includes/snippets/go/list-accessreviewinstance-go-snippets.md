---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ccf72438c92b4021e6eedbcdbcb93032df33f5eb
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61086256"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.InstancesRequestBuilderGetQueryParameters{
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.InstancesRequestBuilderGetOptions{
    Q: requestParameters,
}
accessReviewScheduleDefinitionId := "accessReviewScheduleDefinition-id"
result, err := graphClient.IdentityGovernance().AccessReviews().DefinitionsById(&accessReviewScheduleDefinitionId).Instances().Get(options)


```