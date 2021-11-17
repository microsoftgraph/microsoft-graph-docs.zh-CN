---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 443f820aaad96a1b467f7bfc5c9e35eef5490a42
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "61029266"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestParameters := &msgraphsdk.SecureScoresRequestBuilderGetQueryParameters{
    Top: 1,
}
options := &msgraphsdk.SecureScoresRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Security().SecureScores().Get(options)


```