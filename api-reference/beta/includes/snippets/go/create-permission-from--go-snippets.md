---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f6f5de95772b22dc2482f66ca3a4634d017219bf
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65327424"
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
    SetAdditionalData(map[string]interface{}{
    }
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Permissions().Post(requestBody)


```