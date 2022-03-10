---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: f9fe1020beff734d158b0ede2452a1fb9ef02d4b
ms.sourcegitcommit: dfa87904fb26dd5161f604f2716ce1d90dad31ed
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/09/2022
ms.locfileid: "63412537"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "Catalog One"
requestBody.SetDisplayName(&displayName)
options := &msgraphsdk.AccessPackageCatalogRequestBuilderPatchOptions{
    Body: requestBody,
}
accessPackageCatalogId := "accessPackageCatalog-id"
result, err := graphClient.IdentityGovernance().EntitlementManagement().CatalogsById(&accessPackageCatalogId).Patch(options)


```