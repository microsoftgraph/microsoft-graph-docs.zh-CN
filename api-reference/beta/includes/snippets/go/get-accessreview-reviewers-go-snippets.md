---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f8d8eb4b91b04452e43c48419a35b2ffcd37c36f
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61089577"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

accessReviewId := "accessReview-id"
result, err := graphClient.AccessReviewsById(&accessReviewId).Reviewers().Get(options)


```