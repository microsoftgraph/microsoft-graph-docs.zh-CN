---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: eec672516157547272f070a7e01ab3ea2b342889
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65325900"
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
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackages().Post(requestBody)


```