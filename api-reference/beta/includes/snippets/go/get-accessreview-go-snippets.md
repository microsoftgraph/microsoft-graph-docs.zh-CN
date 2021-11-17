---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: d9b2f200d273eae4063020ebe7740b9b9f86c48e
ms.sourcegitcommit: a6cbea0e45d2e84b867b59b43ba6da86b54495a3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/16/2021
ms.locfileid: "60988138"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter);

accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Get(options)


```