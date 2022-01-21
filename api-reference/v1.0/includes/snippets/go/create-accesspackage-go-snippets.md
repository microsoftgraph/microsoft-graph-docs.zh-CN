---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: ce25a32e6a6b04db056f5c3a27c59b3832bfd96c
ms.sourcegitcommit: a16b765507093d892022603d521c0ae8043de432
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/20/2022
ms.locfileid: "62100948"
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
id := "66584aae-98bb-48cc-9458-7bee5d2a6577"
catalog.SetId(&id)
options := &msgraphsdk.AccessPackagesRequestBuilderPostOptions{
    Body: requestBody,
}
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackages().Post(options)


```