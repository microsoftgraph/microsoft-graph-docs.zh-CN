---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 2b6326a641ab1722b4b41af90ebdf13fcc125bb2
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66094911"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewEdiscoverySearch()
displayName := "My search 2"
requestBody.SetDisplayName(&displayName)
description := "My first search"
requestBody.SetDescription(&description)
contentQuery := "(Author="edison")"
requestBody.SetContentQuery(&contentQuery)
requestBody.SetAdditionalData(map[string]interface{}{
    "custodianSources@odata.bind":  []String {
        "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/userSources/43434642-3137-3138-3432-374142313639",
        "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/custodians/0053a61a3b6c42738f7606791716a22a/siteSources/169718e3-a8df-449d-bef4-ee09fe1ddc5d",
        "https://graph.microsoft.com/beta/security/cases/ediscoveryCases('b0073e4e-4184-41c6-9eb7-8c8cc3e2288b')/custodians('0053a61a3b6c42738f7606791716a22a')/unifiedGroupSources('32e14fa4-3106-4bd2-a245-34bf0c718a7e')",
    }
    "noncustodialSources@odata.bind":  []String {
        "https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/noncustodialdatasources/35393639323133394345384344303043",
    }
}
ediscoveryCaseId := "ediscoveryCase-id"
result, err := graphClient.Security().Cases().EdiscoveryCasesById(&ediscoveryCaseId).Searches().Post(requestBody)


```