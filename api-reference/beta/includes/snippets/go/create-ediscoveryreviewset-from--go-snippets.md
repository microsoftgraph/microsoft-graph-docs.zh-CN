---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0842d23d1dd2ce2f80a25f81802ec6fa30c4963e
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095198"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryReviewSet()
displayName := "My review set 2"
requestBody.SetDisplayName(&displayName)
ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).ReviewSets().Post(requestBody)


```