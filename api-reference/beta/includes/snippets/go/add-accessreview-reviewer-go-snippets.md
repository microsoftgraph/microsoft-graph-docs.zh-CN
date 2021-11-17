---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 5288685cef41caa3e4a0cb4aa3d1220ac6ba2da3
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988173"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

requestBody := msgraphsdk.NewAccessReviewReviewer()
id := "006111db-0810-4494-a6df-904d368bd81b"
requestBody.SetId(&id)
options := &msgraphsdk.ReviewersRequestBuilderPostOptions{
    Body: requestBody,
}
accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Reviewers().Post(options)


```