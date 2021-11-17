---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: aed958bb5a5c715e7b9d182ed8c78056ad7e3a1e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987838"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

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