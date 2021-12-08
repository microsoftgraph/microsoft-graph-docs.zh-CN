---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: 99f2250b7c05ebf12abb8cb4c112ce5af8a7f749
ms.sourcegitcommit: 65f4e128f96783c18d607a6dcffbc914291285d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/08/2021
ms.locfileid: "61341812"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackage()
displayName := "sales reps"
requestBody.SetDisplayName(&displayName)
description := "outside sales representatives"
requestBody.SetDescription(&description)
isHidden := false
requestBody.SetIsHidden(&isHidden)
catalog := msgraphsdk.NewAccessPackageCatalog()
requestBody.SetCatalog(catalog)
catalog.SetAdditionalData(map[string]interface{}{
    "id": "66584aae-98bb-48cc-9458-7bee5d2a6577",
}
options := &msgraphsdk.AccessPackagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackages().Post(options)


```