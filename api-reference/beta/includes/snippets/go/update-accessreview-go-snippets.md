---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 71f0281bd3d8e8162f71621c28fdeeea1f888f44
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394192"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReview()
displayName := "TestReview new name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessReviewRequestBuilderPatchOptions{
    Body: requestBody,
}
accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Patch(options)


```