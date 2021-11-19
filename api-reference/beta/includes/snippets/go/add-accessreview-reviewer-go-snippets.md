---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ff845156d57d73a80156d99bd1679009145203f9
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61087899"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReviewReviewer()
id := "006111db-0810-4494-a6df-904d368bd81b"
requestBody.SetId(&id)
options := &msgraphsdk.ReviewersRequestBuilderPostOptions{
    Body: requestBody,
}
accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Reviewers().Post(options)


```