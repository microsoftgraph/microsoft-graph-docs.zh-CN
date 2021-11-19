---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d6cacbf18b9a432f315bcd59e5f86ad3162035fd
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101919"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestParameters := &msgraphsdk.SecureScoresRequestBuilderGetQueryParameters{
    Top: 1,
}
options := &msgraphsdk.SecureScoresRequestBuilderGetOptions{
    Q: requestParameters,
}
result, err := graphClient.Security().SecureScores().Get(options)


```