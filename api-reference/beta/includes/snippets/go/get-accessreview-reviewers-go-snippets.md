---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0e87b43b3460361ed3c01d58f51efa93255bb387
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988040"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Reviewers().Get(options)


```