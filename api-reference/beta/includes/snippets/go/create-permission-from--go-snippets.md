---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 7c2f46073e8ccb438a5d0daa87efcba70fdb60ef
ms.sourcegitcommit: 2456cf3c4117b88afefef139593796a2f919e7cc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2021
ms.locfileid: "61101474"
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
options := &msgraphsdk.PermissionsRequestBuilderPostOptions{
    Body: requestBody,
}
siteId := "site-id"
result, err := graphClient.SitesById(&siteId).Permissions().Post(options)


```