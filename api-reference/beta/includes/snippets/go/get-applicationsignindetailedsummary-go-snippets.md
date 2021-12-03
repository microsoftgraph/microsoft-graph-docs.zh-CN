---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 158560a60afc24b3dd4702c9b33094c89fd4ac55
ms.sourcegitcommit: b16e230f4347f23d8e1bda0681daa93025a39a6d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2021
ms.locfileid: "61287555"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

applicationSignInDetailedSummaryId := "applicationSignInDetailedSummary-id"
result, err := graphClient.Reports().ApplicationSignInDetailedSummaryById(&applicationSignInDetailedSummaryId).Get(nil)


```