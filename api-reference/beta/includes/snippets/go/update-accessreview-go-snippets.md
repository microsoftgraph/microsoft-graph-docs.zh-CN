---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: da19379952cd21ac6abf406baa945e1bcd3d4170
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61085700"
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
graphClient.AccessReviewsById(&accessReviewId).Patch(options)


```