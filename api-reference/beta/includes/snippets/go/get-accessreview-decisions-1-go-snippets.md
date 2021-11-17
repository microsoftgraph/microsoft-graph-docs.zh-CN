---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: fd15bb5f0afd6f84f33d1598c9737b41630963ac
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988096"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Decisions().Get(options)


```