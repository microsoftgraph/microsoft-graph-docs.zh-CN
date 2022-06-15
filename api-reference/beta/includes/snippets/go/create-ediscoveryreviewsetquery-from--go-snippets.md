---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 51762395a6c3e55c0462de4d34b61feaacc92d0c
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094680"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryReviewSetQuery()
displayName := "My Query 1"
requestBody.SetDisplayName(&displayName)
contentQuery := "(Author="edison")"
requestBody.SetContentQuery(&contentQuery)
ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewSetId := "ediscoveryReviewSet-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).ReviewSetsById(&ediscoveryReviewSetId).Queries().Post(requestBody)


```