---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: b7697ea94652295f5ca6234b3c214f080351f9a9
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66093492"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryCustodian()
email := "AdeleV@contoso.com"
requestBody.SetEmail(&email)
ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Custodians().Post(requestBody)


```