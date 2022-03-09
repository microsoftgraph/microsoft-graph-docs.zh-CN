---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: e8336ec136da3b7e9b6971f249c2039e23d774df
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63394178"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
accessReviewReviewerId := "accessReviewReviewer-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).ReviewersById(&accessReviewReviewerId).Delete(nil)


```