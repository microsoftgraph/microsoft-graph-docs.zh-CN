---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 96bd36e7fb5b7222c2ed8bc4ba1ab932cb42ee97
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60987999"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessReview()
displayName := "TestReview new name"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessReviewRequestBuilderPatchOptions{
    Body: requestBody,
}
accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).Patch(options)


```