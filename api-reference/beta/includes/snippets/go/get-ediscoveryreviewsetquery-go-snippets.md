---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 4487287685df324bdee6d03567403350a471711d
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095435"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

ediscoveryCaseId := "ediscoveryCase-id"
ediscoveryReviewSetId := "ediscoveryReviewSet-id"
ediscoveryReviewSetQueryId := "ediscoveryReviewSetQuery-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).ReviewSetsById(&ediscoveryReviewSetId).QueriesById(&ediscoveryReviewSetQueryId).Get()


```