---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 63f08c94024282c49fe8f09e51946a28d82398d7
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60979767"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.DefinitionsRequestBuilderGetQueryParameters{
    Filter: "contains(scope/microsoft.graph.accessReviewQueryScope/query,%20'./members')",
}
options := &msgraphsdk.DefinitionsRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.IdentityGovernance().AccessReviews().Definitions().Get(options)


```