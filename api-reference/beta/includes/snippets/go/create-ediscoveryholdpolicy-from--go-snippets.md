---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 0106851e889099677ac30c470e16034d584673eb
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66096132"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoveryHoldPolicy()
displayname := "My legalHold with sources"
requestBody.SetDisplayname(&displayname)
description := "Created from Graph API"
requestBody.SetDescription(&description)
contentQuery := "Bazooka"
requestBody.SetContentQuery(&contentQuery)
requestBody.SetAdditionalData(map[string]interface{}{
    "userSources@odata.bind":  []Object {
    }
    "siteSources@odata.bind":  []Object {
    }
}
ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).LegalHolds().Post(requestBody)


```