---
description: 自动生成文件。 请不要修改
ms.openlocfilehash: c9221de560081bc930ff4692388d22fe57a0a3c2
ms.sourcegitcommit: 30d1f0d898b6e4488d1938251fba143370119241
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2022
ms.locfileid: "65326375"
---
```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)

requestBody := msgraphsdk.NewAccessPackageCatalog()
displayName := "sales"
requestBody.SetDisplayName(&displayName)
description := "for employees working with sales and outside sales partners"
requestBody.SetDescription(&description)
isExternallyVisible := true
requestBody.SetIsExternallyVisible(&isExternallyVisible)
result, err := graphClient.IdentityGovernance().EntitlementManagement().AccessPackageCatalogs().Post(requestBody)


```