---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 81bca8699bc5cde7ad9a05946aca8267c00d3f53
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63411699"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
graphClient.AccessReviewsById(&accessReviewId).ApplyDecisions(accessReview-id).Post(nil)


```