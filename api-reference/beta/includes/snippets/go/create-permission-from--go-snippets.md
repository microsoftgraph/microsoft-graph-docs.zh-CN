---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 265d2dfffc7e46a2fe4ac7e47b793d2da473ad16
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/15/2022
ms.locfileid: "66098743"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewPermission()
requestBody.SetRoles( []String {
    "write",
}
requestBody.SetGrantedToIdentities( []IdentitySet {
    msgraphsdk.NewIdentitySet(),
application := msgraphsdk.NewIdentity()
    SetApplication(application)
id := "89ea5c94-7736-4e25-95ad-3fa95f62b66e"
    application.SetId(&id)
displayName := "Contoso Time Manager App"
    application.SetDisplayName(&displayName)
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Permissions().Post(requestBody)


```