---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 9988da3f25c1742e667b284aaa06a03a66fd4707
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326186"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessReview()
displayName := "TestReview new name"
requestBody.SetDisplayName(&displayName)
accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).Patch(requestBody)


```