---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5ee9ca825fbeeb5ed5a9e4c67f5245007c2fd123
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60991870"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.PendingAccessReviewInstancesRequestBuilderGetQueryParameters{
    Expand: "definition",
    Top: 100,
    Skip: 0,
}
options := &msgraphsdk.PendingAccessReviewInstancesRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Me().PendingAccessReviewInstances().Get(options)


```